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

## TC_REGISTRATION_004 — Registration fails with invalid phone number (shorter than 10 characters)

### Feature
Employee Registration Form

### Priority
High

### Severity
High

### Preconditions
- User is logged into the system with HR admin permissions
- User has access to Employee Registration module
- User is on the Employee Registration form page

### Test Data
1. Phone number: 1234567
2. Remaining fields: valid data

### Steps to Reproduce
1. Log in to the system with HR admin credentials
2. Navigate to Employee Registration page
3. Enter "1234567" in Phone Number field
4. Fill the rest of the fields with valid data
5. Click on "submit"

### Expected Result
- Employee is not registered
- Validation error message should be displayed for Phone Number field
- System should reject invalid Phone Number input
- Employee data should not be added to the table

### Actual Result
- Employee is registered
- No validation error message is displayed for the Phone Number field
- Invalid Phone Number value ("1234567") is accepted

### Status
Fail

---

## TC_REGISTRATION_005 — Registration fails with inconsistent Age and Date of Birth

### Feature
Employee Registration Form

### Priority
High

### Severity
Critical

### Test Data
- Age: 25
- Date of Birth: 21/07/2005
- Remaining fields: valid data

### Steps to Reproduce
1. Log in to the system with HR admin credentials
2. Navigate to Employee Registration page
3. Enter "25" in Age field
4. Enter "21/07/2005" in Date of Birth field
5. Fill the remaining fields with valid data
6. Click on "Submit"

### Expected Result
- Employee should not be registered
- System should validate consistency between Age and Date of Birth
- Validation error message should be displayed

### Actual Result
- Employee is registered
- No validation error is displayed
- System accepts inconsistent data

### Status
FAIL
---

## TC_REGISTRATION_006 - Registration fails with wrong form of data in Age field

### Feature
Employee Registration Form

### Priority
Medium

### Severity
Medium

### Preconditions
- User is logged into the system with HR admin permissions
- User has access to Employee Registration module
- User is on the Employee Registration form page

### Test data
1. Age: Twenty-Five
2. Remaining fields: valid data

### Steps to Reproduce
1. Log in to the system with HR admin credentials
2. Navigate to Employee Registration page
3. Enter "Twenty-Five" in Age field
4. Fill the rest of the fields with valid data
5. Click on "submit"

### Expected Result
- User should not be able to fill Age field with non numeric characters
- Therefore, employee should not be registered

### Actual Result
- User cannot fill Age field with non numeric characters
- Employee data is not registered

### Status
Pass

---

## TC_REGISTRATION_007 - Registration fails with negative value in Expected Salary field

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
1. Expected Salary: -30000
2. Remaining fields: valid data

### Steps to Reproduce
1. Log in to the system with HR admin credentials
2. Navigate to Employee Registration page
3. Enter "-30000" in Expected Salary field
4. Fill the rest of the fields with valid data
5. Click on "submit"

### Expected Result
- Employee should not be registered
- Validation error message should be displayed for Expected Salary field
- System should reject all values lower than 0 for the Expected Salary field

### Actual Result
- Employee is registered
- No validation error message is shown
- System accepts values lower than 0 for the Salary field

### Status 
Fail

---

## TC_REGISTRATION_008 - Registration fails with values out of the accepted range for Age field

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

### Test data
1. Age: Any value between 5-17 (e.g., "15")
2. Remaining fields: valid data

### Steps to Reproduce
1. Log in to the system with HR admin credentials
2. Navigate to Employee Registration page
3. Enter any value between 5-17 (e.g., "15") in Age field
4. Fill the remaining fields with valid data
5. Click on "submit"

### Expected Result
- System should not allow any value outside of the accepted range in Age field
- Validation error message should be displayed
- Employee should not be registered

### Actual Result
- System allows user to fill Age field with values outside the accepted range, specifically any value between 5 and 17
- No validation error message is displayed
- Employee is registered

### Status
Fail

---

## TC_REGISTRATION_009 — Registration behavior at boundary values for Age field

### Feature
Employee Registration Management

### Priority
High

### Severity
Critical

### Test Data
- Age: 18 and 65
- Remaining fields: valid data

### Steps to Reproduce
1. Log in to the system with HR admin credentials
2. Navigate to Employee Registration page
3. Enter "18" in Age field and complete form
4. Submit the form
5. Repeat with "65" in Age field

### Expected Result
- Employee should be registered successfully with both values
- System should accept boundary values (18 and 65)

### Actual Result
- Age "18" works correctly
- Age "65" is rejected
- Error message contradicts validation rules

### Status
FAIL

---

## TC_REGISTRATION_010 - Registration fails with future dates of birth

### Feature
Employee Registration Form

### Priority
Medium

### Severity
Medium

### Preconditions
- User is logged into the system with HR admin permissions
- User has access to Employee Registration module
- User is on the Employee Registration form page

### Test Data
1. Date of Birth: Any date after current one (e.g., "20/01/2050")
2. Remaining fields: valid data

### Steps to Reproduce
1. Log in to the system with HR admin credentials
2. Navigate to Employee Registration page
3. Enter "20/01/2050" in Date of Birth field
4. Fill the rest of the fields with valid data
5. Click on "submit"

### Expected Result
- Employee should not be registered
- System should reject any date beyond the current one
- Validation error message should be displayed

### Actual Result
- Employee is registered
- System accepts any date of birth
- Employee data is added to the table

### Status
Fail

---

## TC_REGISTRATION_011 - Registration fails with invalid form of Email

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
1. Email: anderramirez.qa
2. Remaining fields: valid data

### Steps to Reproduce
1. Log in to the system with HR admin credentials
2. Navigate to Employee Registration page
3. Enter "anderramirez.qa" in Email field
4. Fill the rest of the fields with valid data
5. Click on "submit"

### Expected Result
- Employee should not be registered
- Validation error message should be displayed for invalid field

### Actual Result
- Employee is not registered
- Validation error message is displayed addressing the issue and indicates fields requirements

### Status
Pass

---

