1. Create a python program for creating a job post in LinkedIn:
code:
from selenium import webdriver
from selenium.webdriver.common.keys import Keys

# Set up the WebDriver (make sure you have installed the appropriate driver for your browser)
driver = webdriver.Chrome()

# Navigate to LinkedIn and log in
driver.get('https://www.linkedin.com')
# Add code to enter your username and password

# Create a job post
driver.get('https://www.linkedin.com/jobs/post/')
# Add code to fill in the job post details (e.g., title, description, location, etc.)

# Submit the job post
submit_button = driver.find_element_by_xpath('//button[@data-control-name="submit_job"]')
submit_button.click()

# Close the browser
driver.quit()


2. Create a web page for creating a job post in Monster:
code:
<!DOCTYPE html>
<html>
<head>
    <title>Create Job Post - Monster</title>
</head>
<body>
    <form method="POST" action="https://www.monster.com/jobs/post">
        <label for="job_title">Job Title:</label>
        <input type="text" id="job_title" name="job_title" required><br><br>

        <label for="job_description">Job Description:</label>
        <textarea id="job_description" name="job_description" required></textarea><br><br>

        <label for="location">Location:</label>
        <input type="text" id="location" name="location" required><br><br>

        <input type="submit" value="Submit">
    </form>
</body>
</html>


3. Create a web page for creating a job post in Hirect:
code:
<!DOCTYPE html>
<html>
<head>
    <title>Create Job Post - Hirect</title>
</head>
<body>
    <form method="POST" action="https://www.hirect.org/create-job-post">
        <label for="job_title">Job Title:</label>
        <input type="text" id="job_title" name="job_title" required><br><br>

        <label for="job_description">Job Description:</label>
        <textarea id="job_description" name="job_description" required></textarea><br><br>

        <label for="location">Location:</label>
        <input type="text" id="location" name="location" required><br><br>

        <input type="submit" value="Submit">
    </form>
</body>
</html>



4. Create an employee attendance sheet using a Python program:

code:
import datetime

# Get the current date and time
current_date = datetime.datetime.now()

# Save the attendance in a file
with open('attendance.txt', 'a') as file:
    file.write(f'{current_date.strftime("%Y-%m-%d %H:%M:%S")}\n')


5. Prepare a leave application using a web page:

code:
<!DOCTYPE html>
<html>
<head>
    <title>Leave Application</title>
</head>
<body>
    <form method="POST" action="/submit_leave_application">
        <label for="employee_name">Employee Name:</label>
        <input type="text" id="employee_name" name="employee_name" required><br><br>

        <label for="leave_reason">Reason for Leave:</label>
        <textarea id="leave_reason" name="leave_reason" required></textarea><br><br>

        <label for="leave_duration">Leave Duration:</label>
        <input type="text" id="leave_duration" name="leave_duration" required><br><br>

        <input type="submit" value="Submit">
    </form>
</body>
</html>


6. Create a web page to generate an employee ID card with BGV QR Code:

code
<!DOCTYPE html>
<html>
<head>
    <title>Employee ID Card</title>
    <style>
        /* CSS styles for the ID card */
        #id_card {
            width: 300px;
            height: 200px;
            border: 1px solid #000;
            padding: 10px;
            text-align: center;
        }

        /* CSS styles for the BGV QR Code */
        .bgv_qr_code {
            width: 100px;
            height: 100px;
            margin-top: 20px;
            background-color: #000;
        }
    </style>
</head>
<body>
    <div id="id_card">
        <h2>Employee ID Card</h2>
        <p>Name: John Doe</p>
        <p>Employee ID: 12345</p>
        <div class="bgv_qr_code"></div>
    </div>
</body>
</html>
