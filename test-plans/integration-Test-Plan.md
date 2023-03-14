# Test Plan for Paul's Lumber Pricing Calculator

### Level of testing
Integration

### Test Objectives
- Validate all documented endpoints work.
  - Correct JSON and status code
- Ensure that the front-end is able to communicate with the backend server without errors.

### Test Approach/Strategy
- Regression-Averse
  - Use an API like Postman tool to ensure test reusability
    - API tests should be stored as a postman collection
- Methodical 
  - [ ] all endpoints return a 200 status code when used correctly
  - [ ] invalid routes return a 404

### Test Basis
- API spec located at [soure](notreal)

### Test Object(s)
- Lumber Pricer Backend  [soure](notreal)
- Lumber Pricer Frontend  [source](notreal)

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
  - [link to exe file](notreal)
- An html web page that contains the pricing calculator
  - [link to repo containing webpage](notreal)
- OpenAPI document listing current endpoints
  - [link](notreal)
- **Test Environment**
  - Testing will be performed on the Tester's local machine
  - The .exe is expected to work on a windows OS

### Exit Criteria
- Postitive tests for all routes have been executed.
- All defect reports are in GitHub
  - [report repo](notreal)
- Test Summary Report completed and in Github
  - [report repo](notreal)
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


### Reporting and Templates
All defects and test reports should be put in this [repo](notreal).Each Defect should be it's own markdown page. There should be one Test Summary report written in markdown. The test summary will be presented to DevOps and Development team.

| Document | Link To Template |
|----------|------|
| Defect Report | [link](notreal) |
| Test Summary | [link](notreal) |
