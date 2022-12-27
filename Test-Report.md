- **Test Report**
  - A document describing how testing is going for a test activity
  - Test Activity could be all unit tests for instance
  - Should include 
    - test metrics
    - Any blockers in testing
    - Progress made related to test plan
     - Summary of tests peformed
    - Comments about the quality of the test object
    - Any deviations from the test plan
  - Should be written with an audience in mind
    - Stakeholder
    - Development team
    - Test Manager
- *Test Progress Report*
  - Report made during testingtesting activity
- *Test Summary Report*
  - Report made at end of testing activity


# Example
In this example the test report is being given to a development team.

## Test Summary of Paul's Lumber Pricing Calculator
The testing team has finsihed performing API tests for the pricing calculator backend. We have focused efforts on verifying the integration functionality between the front-end, back-end and other services which use the service. 

## Tests Performed
- Functional
  - API Testing of the pricing calculator
  - Integration of the backend calculator API with the frontend

## How Tests were performed
- The latest stable build of the [application](notreal) was tested on testers local machines.
- Tests were written in Postman and exported as a collection located [here](notreal)
  - These tests are available for developers to use at anytime in their own regression tests

## Test Results

### API Testing
| route | Test Coverage                |  Note                 |
|-------|------------------------------|-------------------------|
|/calculate | 13/13 Passing            |All tests Passing        |
|/shiftcost | 8/9 Passing              | Failing test is from a typo in response JSON|
|/marketupdate | 0/6 Passing | Numerous defects                  |

### Integration With Frontend website
Exploratory testing by senior testers failed to notice any integration errors with the product. However, the tester did note that calcuations do show many decimal points of precision. Resulting in display values such as $45.8773. This ultimately does not affect the ability of the two pieces to integrate and work.

## Notable Defects
- The /marketupdate routes is intened to use real time data from lumber and wood markets. However all requests made to these routes time out after 10+ seconds. The source of this timeout is related to improperly read environment variables. If these are fixed the application might begin to function as intended.
- The /marketupdate routes do no fail gracefully. Upon timing out or recieving JSONs they cannot parse they spew stacktraces to the screen making a huge security risk. This was not an focus of testing but is significant enough to be an immediate concern.

## Blockers
The defect of incorrect environment variables has prevent the testing team from checking integration with other systems. When it is corrected we can resume testing of that route.

## Overall quality
The application works very quickly and passes almost all tests barring the one route. 

