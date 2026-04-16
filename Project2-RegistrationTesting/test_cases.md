## Project: GeekRetail Registration Testing

# 🧪 Employee Registration Testing - Test Cases

---

## TC_REGISTRATION_001 — Employee is successfully registered with valid data

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
- Schedule: 9am–5pm
- Profile Link: https://github.com/anderramirez-qa
- Expected Salary: 30000

### Steps to Reproduce
1. Log in to the system with HR admin credentials
2. Navigate to Employee Registration page
3. Fill in all required fields with valid data
4. Click on "Submit"

### Expected Result
- Employee is successfully registered
- Success confirmation message is displayed
- Employee information is displayed in the table

### Actual Result
Employee is successfully registered

### Status
PASS

---

## TC_REGISTRATION_002 — Registration fails when mandatory fields are missing

### Feature
Employee Registration Form

### Priority
High

### Severity
Major

### Preconditions
- User is logged into the system with HR admin permissions
- User has access to Employee Registration module
- User is on the Employee Registration form page

### Test Data
- Full Name: (empty)
- Address: (empty)
- Remaining fields: valid data

### Steps to Reproduce
1. Log in to the system with HR admin credentials
2. Navigate to Employee Registration page
3. Leave "Full Name" and "Address" fields empty
4. Fill the rest of the fields with valid data
5. Click on "Submit"

### Expected Result
- Employee should not be registered
- Validation error messages should be displayed for required fields
- Employee data should not be added to the table

### Actual Result
Employee is not registered and validation error messages are displayed

### Status
PASS

---

## TC_REGISTRATION_003 — Registration fails with invalid data in Name and Age fields

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
- Remaining fields: valid data

### Steps to Reproduce
1. Log in to the system with HR admin credentials
2. Navigate to Employee Registration page
3. Enter "123" in Full Name field
4. Enter "80" in Age field
5. Fill the rest of the fields with valid data
6. Click on "Submit"

### Expected Result
- Employee should not be registered
- Validation error messages should be displayed for invalid fields
- System should reject both invalid Name and Age inputs
- Employee data should not be added to the table

### Actual Result
- Employee is not registered
- Validation error message is displayed for Age field
- Invalid Name value ("123") is accepted

### Status
FAIL
---

## TC_REGISTRATION_004 —
