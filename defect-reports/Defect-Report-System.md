```markdown
## Invalid Password wrongfully accepted

#### ID: {number}

#### Status: {OPEN | CLOSED | DEFERRED}

### Summary
{brief summary}

|Expected Behavior | Actual Behavior|
|------------------|----------------|
|                  |                |

### Discovered By
{tester}

### Discovery Date
{mm/dd/yyyy}

### Test Object
{Test Object. Maybe a link to the code or application}

### Steps to reproduce
1. {numbered steps}

### Supporting Evidence
{screenshots and stacktraces}

### Priority
{LOW | MEDIUM | HIGH}

### Severity
{LOW | MEDIUM | HIGH}

### Test Cases Affected
{List of test cases affected}

### Suggestions
{Any possible suggestions of hints to fix it}
```

# Example 

## Invalid Password wrongfully accepted

#### ID: DF101

#### Status: Open

### Summary
A user can login using an invalid password. 

|Expected Behavior | Actual Behavior|
|------------------|----------------|
| User is given a popup saying invalid password | The user is taken to the home page|

### Discovered By
Adam Ranieri

### Discovery Date
3/17/2022

### Test Object
Employee PTO Signup Portal

### Steps to reproduce
1. Navigate to home page
2. input a valid username
3. input an invalid password
4. click submit

### Supporting Evidence
![stacktrace](https://developer.android.com/static/studio/images/debug/logcat-stacktrace_2x.png)
(this stacktrace is unrelated but images related to error would go here)

### Priority
Very High

### Severity
Very High

### Test Cases Affected
- TC-236
- TC-301

### Suggestions
The stacktrace on the backend suggests some failure in the server.


