```markdown
## ID: {next number}

### Status: {OPEN | CLOSED | DEFERRED}

### Discovered By
{Author}

### Discovery Date
{mm/dd/yyyy}

### Request Information

| route | method | body |
|-------|--------|------|
|       |        |      |

### Response Information

|               | Expected   |   Actual  |
|---------------|------------|-----------|
| JSON Response |            |           |
| Status code   |            |           |

### Severity
{HIGH | MEDIUM | LOW}

### Priority
{HIGH | MEDIUM | LOW}

```

# Example

### ID: DF-931

### Status: Open

### Discovered By
John Doe

### Discovery Date
7/27/2022

### Request Information

| route | method | body |
|-------|--------|------|
| /calculate | POST | {"cedar":1}

### Response Information

|          | Expected   |   Actual  |
|----------|------------|-----------|
| JSON Response | {"price":19.50} | ERROR handling request |
| Status code   | 200             | 500                    |

### Severity
- High

### Priority
- High