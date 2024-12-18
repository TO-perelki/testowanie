# TESTPLAN.md

## 1. Introduction

### 1.1 Test Objectives
The primary goal of testing is to ensure the high quality of the Open Food Facts application by verifying its functionality, stability, and performance. Testing also aims to identify and eliminate potential bugs before the deployment of new features.

### 1.2 Business Context of the Application
Open Food Facts is an open-source database of food products that allows users to analyze ingredients, nutritional values, and the health impact of products. The platform supports sustainability and informed consumer decisions. For the user community, the reliability and accessibility of data are crucial, making application quality paramount.

### 1.3 Scope of Testing
#### Functionalities:
- Searching for products using barcodes (REQ-FUNC-001).
- Viewing detailed product ingredient information (REQ-FUNC-002).
- Sorting search results by various criteria (REQ-FUNC-003).
- Adding new products to the database (REQ-FUNC-004).
- Displaying allergen and dietary preference information (REQ-FUNC-005, REQ-FUNC-009).
- Supporting multiple interface languages (REQ-FUNC-006).
- Reporting incorrect or incomplete data (REQ-FUNC-007).
- Displaying health ratings of products (REQ-FUNC-008).
- Response time below 2 seconds for queries (REQ-NFUNC-001).
- Recognizing barcodes within 1 second (REQ-NFUNC-002).

#### Types of Testing:
- Functional testing.
- Performance testing.
- Regression testing.

---

## 2. Testing Goals and Criteria

### 2.1 Entry Criteria
- The application code is stable and available in the designated version.
- Documentation of functional and non-functional requirements (REQ-FUNC and REQ-NFUNC) is complete.
- A test environment and test data are available.
- Testing team members and technical roles are assigned.

### 2.2 Exit Criteria
- All planned test cases are executed.
- No critical or high-risk bugs remain.
- Final test report is approved by the project team.

### 2.3 Acceptance Criteria for Test Results
- All functional requirements (REQ-FUNC-001 to REQ-FUNC-009) have been verified, with tests accepted and functionalities working as expected.
- Performance tests: response times do not exceed 1 second for 95% of requests.
- The number of medium and low-priority bugs is deemed acceptable and does not affect key application functionality.
- Regression tests: no regressions in functionality after new features are implemented.

---

## 3. Testing Strategy

### 3.1 Testing Approach
- Tests will be conducted in iterative cycles, covering different types of tests.
- Functional tests will verify compliance with business requirements.
- Performance tests will assess system response times and stability under load.

### 3.2 Types of Tests
- **Functional Tests:** Verification of key application functionalities.
- **Non-functional Tests:** Performance testing.
- **Regression Tests:** Ensuring that changes do not negatively impact existing functionality.

### 3.3 Tools and Testing Environment
- **Tools:**
  - Selenium WebDriver – for browser test automation.
  - JMeter – for performance testing.
- **Environment:**
  - Test servers with access to the latest version of the application.
  - Test data from the Open Food Facts database.

---

## 4. Schedule and Resources

### 4.1 Testing Schedule

- **November (Week 2):** Introduce teams, members, tasks, identified risks, and the FOSS application.  
- **November (Week 3):** Present requirement specifications.  
- **November (Week 4):** Present test plans.  
- **December (Week 1):** Iteration 1: Prepare high-level test cases for each area.  
- **December (Week 2):** Iteration 2: Refine cases (add steps, test data), prepare a pool for the second team, and assign teams for cross-testing.  
- **December (Week 3):** Iteration 1 Results: Present test results (REQ-FUNC-001 to REQ-FUNC-005) tested by another team.  
- **December (Week 4):** Iteration 2 Results: Present results of own tests (REQ-FUNC-001 to REQ-FUNC-005).  
- **January (Week 1):** Iteration 3 Results: Present results of tests (REQ-FUNC-006 to REQ-FUNC-009, REQ-NFUNC-001 to REQ-NFUNC-002).  
- **January (Week 2):** Iteration 4 Results: Present results of tests (REQ-FUNC-006 to REQ-FUNC-009, REQ-NFUNC-001 to REQ-NFUNC-002).  
- **January (Week 3):** Final Reports: Present results and a one-page summary.  
- **January (Week 4):** Buffer Time: Address any final adjustments or missing elements.  

### 4.2 Roles and Responsibilities
| Role                  | Person           | Responsibilities                                                |
|-----------------------|------------------|----------------------------------------------------------------|
| Test Manager          | Kacper and Oliwia | Test planning and management.                                   |
| Functional Tester     | Kacper and Oliwia | Testing compliance with requirements.                          |
| Performance Tester    | Kacper and Oliwia | Evaluating application performance.                            |
| Regression Tester     | Kacper and Oliwia | Verifying that changes do not negatively impact functionality. |

---

## 5. Risk Management - Potential Risks, Impact, and Mitigation Plans

1. **Lack of access to the testing environment**  
   - **Impact:** Delays in test execution.  
   - **Mitigation Plan:** Regular communication with the development team to ensure environment availability.  

2. **Incomplete requirements**  
   - **Impact:** Improper preparation of test cases.  
   - **Mitigation Plan:** Verify requirements before starting testing to ensure completeness.  

3. **Critical bugs detected too late**  
   - **Impact:** Deployment delays.  
   - **Mitigation Plan:** Close collaboration with the development team for ongoing fixes.  

4. **Incomplete test data**  
   - **Impact:** May affect test results.  
   - **Mitigation Plan:** Prepare backup copies of test data and verify them before use.  

5. **Unexpected code changes**  
   - **Impact:** May require additional tests.  
   - **Mitigation Plan:** Regularly monitor code changes and synchronize with the development team.  

6. **Lack of experience with open-source application testing**  
   - **Impact:** Hinders effective testing.  
   - **Mitigation Plan:** Familiarize with open-source project practices and consult experienced team members.  

7. **Insufficient time resources**  
   - **Impact:** Inability to test all functionalities.  
   - **Mitigation Plan:** Prioritize tests and plan activities realistically, considering available time resources.  

---

## 6. Metrics and Reporting

### 6.1 Key Quality Indicators
- Percentage of test cases executed successfully.
- Number of critical bugs detected.
- Bug resolution time.
- Average response time (performance).

### 6.2 Reporting Test Results
- Progress Reports:
  - Summary of completed tests, detected bugs, and schedule progress.
  - Number of test cases executed and passed.
  - Number of bugs detected.
  - Bug status (new, resolved, reopened).
- Final Report:
  - Number of bugs by priority.
  - Performance test results:
    - **Average response time:** The average time the system takes to process user requests from submission to response.
    - **95% response time:** The time within which 95% of all tested requests receive a response.
  - Evaluation of compliance with acceptance criteria.
