const axios = require('axios');
const cheerio = require('cheerio');
const XLSX = require('xlsx');

// URL of Yoshops.com page to scrape
const url = 'https://www.yoshops.com';

axios.get(url)
  .then(response => {
    // Load the HTML content into Cheerio
    const $ = cheerio.load(response.data);

    // Extract the desired data from the website using appropriate selectors
    // Replace the selectors below with the ones specific to Yoshops.com
    const productNames = $('.product-name').map((_, element) => $(element).text()).get();
    const productDetails = $('.product-details').map((_, element) => $(element).text()).get();
    const productReviews = $('.product-review').map((_, element) => $(element).text()).get();
    const customerNames = $('.customer-name').map((_, element) => $(element).text()).get();
    const customerEmails = $('.customer-email').map((_, element) => $(element).text()).get();

    // Create a data array from the extracted data
    const data = [
      ['Product Name', 'Product Details', 'Product Review', 'Customer Name', 'Customer Email'],
      ...productNames.map((name, index) => [name, productDetails[index], productReviews[index], customerNames[index], customerEmails[index]])
    ];

    // Create a new workbook and sheet using SheetJS
    const workbook = XLSX.utils.book_new();
    const sheet = XLSX.utils.aoa_to_sheet(data);

    // Add the sheet to the workbook
    XLSX.utils.book_append_sheet(workbook, sheet, 'Yoshops Data');

    // Write the workbook to a file
    XLSX.writeFile(workbook, 'yoshops_data.xlsx');
  })
  .catch(error => {
    console.error('Error:', error);
  });
