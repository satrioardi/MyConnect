# 🚀 **Quality Assurance Tester - Automation Testing**

Welcome to my take-home test submission for the **Quality Assurance Tester** position at **MyConnect.ai**. Below is a detailed overview of the tasks and the solutions I have implemented.

---

## 📝 **Table of Contents**
1. [Task 1: End-to-End (E2E) Automation Testing](#task-1)
2. [Task 2: API Automation Testing](#task-2)
3. [Task 3: Load and Performance Testing](#task-3)
4. [Execution and Setup](#execution-and-setup)
5. [Conclusion](#conclusion)

---

## ⚙️ **Task 1: End-to-End (E2E) Automation Testing (Playwright)**

### **Overview**
For Task 1, I implemented E2E tests for user authentication using **Playwright**. The test cases cover valid and invalid login scenarios, along with testing a wrong password input.

### **Test Cases Implemented**
1. **Valid User Login:**
   - Scenario: A user logs in with valid credentials.
   - Action: Username: `kminchelle`, Password: `0lelplR`.
   - Expected Result: User is redirected to the dashboard with a welcome message or token.
   
2. **Invalid User Login (User Not Found):**
   - Scenario: A user tries to log in with an invalid username.
   - Action: Username: `invalidUser`, Password: `wrongPassword`.
   - Expected Result: Login attempt fails with an appropriate error message.
   
3. **Wrong Password Test:**
   - Scenario: A user enters the correct username but provides the wrong password.
   - Action: Username: `kminchelle`, Password: `wrongPassword`.
   - Expected Result: Login attempt fails with an appropriate error message.

### **Test Execution**
- To run the test, clone the repository and install the dependencies by running:
  ```bash
  npm install
