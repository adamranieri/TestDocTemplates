Often Unit tests are automated and conducted by the developer using an automated testing frameworks. Unit testing defect reports are uncommon.

```markdown

## ID {number}

### Summary
{description}

### Discovered By
{Author}

### Discovery Date
{mm/dd/yyyy}

### Code Location
{link to file in version control}

### Method Signature
{Code snippet}

|Input             | Expected Output  | Acutal Output  |
|------------------|------------------|----------------|
|                  |                  |                |

### Supporting Evidence
{stacktrace if applicable}

### Severity
- High

### Priority
- High
```
# Example

## ID 001

### Summary
An input of 0 is treated the same as no input. 

### Discovered By
Bobby McTest

### Discovery Date
09/28/2022

### Code Location
[code file](notreal)

### Method Signature
```python 
def multi_string(phrase: str, times: int) -> str:
```

|Input             | Expected Output  | Acutal Output  |
|------------------|------------------|----------------|
|    multi_string("hello", 0)              |      ""            |     "hello"           |

### Supporting Evidence
No error but a wrongful answer is given

### Severity
- Medium

### Priority
- low