## Project: GeekRetail Registration Testing

# 🧪 Employee Registration Testing - Test Cases

---

## TC_REGISTRATION_001 — Employee is registered with valid data

### Feature
Employee Registration Form

### Priority
High

### Severity
Critical

### Preconditions
- User is logged into the system with HR admin permissions
- User has access to Employee Registration module
- User is on the Employee Registration form page

### Test Data
- Full Name: Ander Ramirez
- Age: 25
- Date of Birth: 21/07/2000
- Gender: Male
- Address: Calle Izaro 16
- Email: anderramirez.qa@gmail.com
- Phone Number: +3464026033
- Job Title: QA Tester
- Department: Logistics
- Contract Status: Active
- Schedule: 9am-17pm
- Profile Link: https://github.com/anderramirez-qa
- Expected Salary: 30.000

### Steps to Reproduce
1. Log in into the system with HR admin permissions
2. Open Employee Registration form
3. Enter valid data in all required fields

### Expected Result
- Employee is registered successfuly
- Success confirmation message is displayed
- Employee's information is visible on the chart

### Actual Result
Employee is registered successfully

### Status
PASS

---

## TC_REGISTRATION_002 — Employee is registered with missing data

### Feature
Employee Registration Form

### Priority
High

### Severity
Critical

### Preconditions
- User is logged into the system with HR admin permissions
- User has access to Employee Registration module
- User is on the Employee Registration form page

### Test Data
- Age: 25
- Date of Birth: 21/07/2000
- Gender: Male
- Email: anderramirez.qa@gmail.com
- Phone Number: +3464026033
- Job Title: QA Tester
- Department: Logistics
- Contract Status: Active
- Schedule: 9am-17pm
- Expected Salary: 30.000

### Steps to Reproduce
1. Log in into the system with HR admin permissions
2. Open Employee Registration form
3. Fill all mandatory fields except "Name" and "Address" fields

### Expected Result
- Employee cannot be registered
- Error message is displayed indicating registration requirements
- Employee's information is not reflected on the chart

### Actual Result
Employee is not registered and error messages are displayed

### Status
PASS

---

## TC_REGISTRATION_003 — Employee is registered with invalid data

### Feature
Employee Registration Form

### Priority
High

### Severity
Critical

### Preconditions
- User is logged into the system with HR admin permissions
- User has access to Employee Registration module
- User is on the Employee Registration form page

### Test Data
- Full Name: 123
- Age: 80
- Date of Birth: 21/07/2000
- Gender: Male
- Adress: Calle Izaro 16
- Email: anderramirez.qa@gmail.com
- Phone Number: +3464026033
- Job Title: QA Tester
- Department: Logistics
- Contract Status: Active
- Schedule: 9am-17pm
- Profile Link: https://github.com/anderramirez-qa
- Expected Salary: 30.000

### Steps to Reproduce
1. Log in into the system with HR admin permissions
2. Open Employee Registration form
3. Enter inavild data in "Name" and "Age" fields
4. Fill the rest of mandatory fields with valid data

### Expected Result
- Employee cannot be registered
- Erorr messages are displayed indicating fields requirements
- Employee's information is not shown on the chart

### Actual Result
Employee is not registered and error message is shown on the "Age" field. However wrong name data is accepted

### Status
Fail

---
