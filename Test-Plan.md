## Test Plan
- The Test Plan is a living document
  - it is *supposed* to be created and alterted as the project and tested evolves
- There might be a master test plan
  - There could be a test plan for each level
- Things included in a test plan
  - Test Objectives
  - *Approach of testing*/ *Test Strategy* 
  - How to integrate testing into the software development lifecycle
  - What to test 
  - How to test
  - Who is doing the test
  - Testing schedule
  - Metrics for monitoring test progress
  - Providing templates to be used for reporting, constructing tests, reporting tests etc...
  - Entry and exit criteria

# Example
---------------------------
# Test Plan for Paul's Lumber Pricing Calculator

### Level of testing
Integration

### Test Objectives
- Validate all documented endpoints work.
  - Correct JSON and status code
- Ensure that the front-end is able to communicate with the backend server without errors.

### Test Approach
- Regression-Averse
  - Use an API like Postman tool to ensure test reusability
    - API tests should be stored as a postman collection
- Methodical 
  - [ ] all endpoints return a 200 status code when used correctly
  - [ ] invalid routes return a 404

### Test Object(s)
- Lumber Pricer Backend
- Lumber Pricer Frontend

### In Scope
- Functional Tests
- Exploratory Tests

### Out of scope
- Non-functional Tests
  - Usability tests
  - Performance
- Functional Testing
  - Mathematical accuracy


### Entry Criteria
- The backend pto service provided as an .exe file
- An html web page that contains the pricing calculator
- **Test Environment**
  - Testing will be performed on the Tester's local machine
  - The .exe is expected to work on a windows OS

### Exit Criteria
- All tests have been executed
- All defect reports are in GitHub
- Test Summary Report completed and in Github
- An exported JSON of the postman collection is in Github

### Test Schedule

| Date  | Milestone|
|-------|----------|
| 12/29 | Test case design Complete |
| 12/30 | Test Execution Complete |
| 12/31 | Test Report and Defects in Github |

### Testers

|Tester | Role | Responsibility |
|-------|------|----------------|
| John  | Lead | Main source of contact for testers |
| Jane  | API Tester | Writing Postman Tests        |
| Mark  | API Tester | Validating documentation against endpoints |


### Document Templates
All defects and test reports should be put in this [repo](notreal).Each Defect should be it's own markdown page. There should be one Test Summary report written in markdown.

#### Defects
