📝 Table of Contents
Task 1: End-to-End (E2E) Automation Testing
Task 2: API Automation Testing
Task 3: Load and Performance Testing
Execution and Setup
Conclusion
⚙️ Task 1: End-to-End (E2E) Automation Testing (Playwright)
Overview
For Task 1, I implemented E2E tests for user authentication using Playwright. The test cases cover valid and invalid login scenarios, along with testing a wrong password input.

Test Cases Implemented
Valid User Login:
Scenario: A user logs in with valid credentials.
Action: Username: kminchelle, Password: 0lelplR.
Expected Result: User is redirected to the dashboard with a welcome message or token.
Invalid User Login (User Not Found):
Scenario: A user tries to log in with an invalid username.
Action: Username: invalidUser, Password: wrongPassword.
Expected Result: Login attempt fails with an appropriate error message.
Wrong Password Test:
Scenario: A user enters the correct username but provides the wrong password.
Action: Username: kminchelle, Password: wrongPassword.
Expected Result: Login attempt fails with an appropriate error message.
Test Execution
To run the test, clone the repository and install the dependencies by running:
bash
Copy
npm install
Execute the tests using the following command:
bash
Copy
npx playwright test
🔌 Task 2: API Automation Testing (Postman & Newman)
Overview
For Task 2, I created and automated the testing of the Login API using Postman and Newman. Below are the various test cases designed to verify different scenarios, such as valid and invalid login, missing passwords, and incorrect username formats.

Test Cases Implemented
Valid Login Test:
Scenario: A valid user credentials are provided.
Expected Result: A valid token is returned.
Invalid Login - User Not Found:
Scenario: An invalid username or non-existent user credentials are provided.
Expected Result: The response should indicate that the user is not found.
Missing Password Test:
Scenario: The password field is left empty.
Expected Result: The API should return an error indicating that the password is required.
Invalid Username Format Test:
Scenario: The username is provided in an incorrect format.
Expected Result: The API should return an error related to invalid username format.
Test Execution
To run the API tests, follow these steps:
Open Postman and import the collection from the postman_collection.json file.
Execute the tests in Postman and verify the results.
For automated execution with Newman (Postman CLI), use the following command:
bash
Copy
newman run postman_collection.json
📊 Task 3: Load and Performance Testing (JMeter)
Overview
For Task 3, I used JMeter to simulate 50 concurrent users logging into the mock API endpoint. The goal was to test the system's ability to handle multiple simultaneous login requests and measure its performance.

Test Plan Structure
Number of Virtual Users: 50 concurrent users.
Duration: 30 seconds to simulate a real-world scenario.
Test Endpoint: https://dummyjson.com/auth/login.
Test Execution
Import the provided JMX file into JMeter.
Start the test by clicking the "Start" button.
JMeter will simulate 50 users, sending login requests to the mock API.
You can view the response times and error rates in the JMeter GUI.
Performance Metrics
Response Times: Monitored for each request made.
Error Rates: Calculated to ensure that the system performs within acceptable limits.
💻 Execution and Setup
Prerequisites
Node.js and npm installed (for Playwright).
Postman and Newman installed (for API Testing).
Apache JMeter installed (for Load Testing).
Steps to Execute the Tests
Clone the repository:
bash
Copy
git clone <repository-link>
cd <repository-folder>
Install the required dependencies:
bash
Copy
npm install
For E2E tests (Playwright):
bash
Copy
npx playwright test
For API tests (Newman):
bash
Copy
newman run postman_collection.json
For Load testing (JMeter):
Import the JMX file into JMeter and run the test plan.
🚀 Conclusion
This project showcases my ability to design and implement automated tests for different types of testing:

End-to-end (E2E) testing using Playwright.
API testing with Postman and Newman.
Load and performance testing with JMeter.
I hope you find my work valuable. If you have any questions or would like further clarification, feel free to reach out!

📚 Additional Information
GitHub Repository: [Insert GitHub Link Here]
Feel free to clone or contribute to this repository as it serves as a template for robust automated testing in real-world scenarios.
