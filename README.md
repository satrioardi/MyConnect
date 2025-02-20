# 🚀 **Quality Assurance Tester - Automation Testing**

Welcome to my take-home test submission for the **Quality Assurance Tester** position at **MyConnect.ai**. Below is a detailed overview of the tasks and the solutions I have implemented.

---

## 📝 **Table of Contents**
1. [Task 1: End-to-End (E2E) Automation Testing](#task-1)
2. [Task 2: API Automation Testing](#task-2)
3. [Task 3: Load and Performance Testing](#task-3)
---

## ⚙️ **Task 1: End-to-End (E2E) Automation Testing (Playwright)**

### **Overview**
For Task 1, I implemented E2E tests for user authentication using **Playwright**. The test cases cover valid and invalid login scenarios, along with testing a wrong password input.

### **Test Cases Implemented**
1. **Valid User Login:**  
2. **Invalid User Login (User Not Found):**   
3. **Wrong Password Test:**

### **Test Execution**
- To run the test, clone the repository and install the dependencies by running:
  ```bash
  npm install
  npx playwright test tests

## ⚙️ **Task 2: EPI Automation Testing (Postman & Newman)**

### **Overview**
For Task 2, I created and automated the testing of the Login API using Postman and Newman. Below are the various test cases designed to verify different scenarios, such as valid and invalid login, missing passwords, and incorrect username formats.

### **Test Cases Implemented**
1. **Valid Login Test:**  
2. **Invalid Login (User Not Found):**   
3. **Missing Password Field Test:**
4. **Invalid Username Format Test:**

### **Test Execution**
-Open Postman and import the collection from the postman_collection.json file.
-Execute the tests in Postman and verify the results.
- For automated execution with Newman (Postman CLI), use the following command
  ```bash
  npm install
  npx playwright test tests

## ⚙️ **Task 3: Load and Performance Testing (JMeter)**
  
### **Overview**
For Task 3, I used JMeter to simulate 50 concurrent users logging into the mock API endpoint. The goal was to test the system's ability to handle multiple simultaneous login requests and measure its performance

### **Test Plan Structure**
1. **Number of Virtual Users: 50 concurrent users.:**  
2. **Duration: 30 seconds to simulate a real-world scenario:**   
3. **Test Endpoint: https://reqres.in/api/login:**

### **Test Execution**
-Import the provided JMX file into JMeter.
-Start the test by clicking the "Start" button.
-JMeter will simulate 50 users, sending login requests to the mock API.
-You can view the response times and error rates in the JMeter GUI.


I hope you find my work valuable. If you have any questions or would like further clarification, feel free to reach out!
