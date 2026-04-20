## Project: GeekRetail Registration Testing

# 🐞 Bug Reports - GeekRetail
Application: https://testing1.geekqa.net/

---

## 🐞 BG001 - Name field accepts invalid data

### Environment
Windows 10, Google Chrome (Version 147.0.7727.56)

### Priority
High

### Severity
Critical

### Description
System allows invalid data such as numbers or just spaces in the Name field.

### Steps to Reproduce
1. Open Employee Registration form
2. Enter spaces or numbers in the Name field
3. Fill the remaining fields with valid data
4. Click on "Submit"

### Expected Result
- Registration should not be completed
- Validation error message should be displayed in the "Name" field indicating the field's requirements

### Actual Result
- System accepts invalid data in the "Name" field
- Employee is registered and added to the table successfully

### Status
Open

---

## 🐞 BG002 - Age field allows values outside the accepted range

### Environment
Windows 10, Google Chrome (Version 147.0.7727.56)

### Priority
High

### Severity
Major

### Description
System accepts values outside the established range (18-65) in the Age field

### Steps to Reproduce
1. Open Employee Registration form
2. Enter "5" in the Age field
3. Fill the remaining fields with valid data
4. Click on "Submit"

### Expected Result
- System should displayed an error message indicating age should be within the established range
- Employee registration should fail

### Actual Result
- System accepts invalid Age data and employee is registered successfully

### Status
Open

---

## 🐞 BG003 - Systems accepts inconsistent Age and Date of Birth

### Environment
Windows 10, Google Chrome (Version 147.0.7727.56)

### Priority
High

### Severity
Critical

### Description
System accepts inconsistent data between Age and Date of Birth fields

### Steps to Reproduce
1. Open Employee Registration form
2. Enter any number in the Age field (e.g., 25)
3. Choose a different date in the Date of Birth field (e.g., 21/07/2010)
4. Fill the remaining fields with valid data
5. Click on "Submit"

### Expected Result
- System should validate consistency between Age and Date of Birth
- Validation error message should be displayed
- Employee should not be registered

### Actual Result
- System accepts inconsistent values for Age and Date of Birth fields
- Employee is registered and added to the table

### Status
Open

---

## 🐞 BG004 - Expected Salary column always displays incorrect value

### Environment
Windows 10, Google Chrome (Version 147.0.7727.56)

### Priority
High

### Severity
Critical

### Description
The Expected Salary column always displays "0" regardless of the value entered

### Steps to Reproduce
1. Open Employee Registration form
2. Enter any valid data in the Expected Salary field (e.g., 30000)
3. Fill the remaining fields with valid data
4. Click on "Submit"

### Expected Result
- Entered salary value should be correctly displayed in the table

### Actual Result
- Expected Salary column always displays "0"

### Status
Open

---

## 🐞 BG005 - Date of Birth field accepts non-existing/future dates

### Environment
Windows 10, Google Chrome (Version 147.0.7727.56)

### Priority
Medium

### Severity
Medium

### Description
Date of Birth field accepts any date, past and future

### Steps to Reproduce
1. Open Employee Registration form
2. Choose any future date in Date of Birth field (e.g., 01/01/2050)
3. Fill the remaining fields with valid data
4. Click on "Submit"

### Expected Result
- The system should not allow the selection of any future or non-existent dates

### Actual Result
- Systems accepts any date, past and future, in the Date of Birth field
- Registration is completed successfully

### Status
Open

---

## 🐞 BG006 - Registration is successful with mandatory data missing

### Environment
Windows 10, Google Chrome (Version 147.0.7727.56)

### Priority
High

### Severity
Critical

### Description
Employee can be registered with empty mandatory fields, such as Gender or Address

### Steps to Reproduce
1. Open Employee Registration form
2. Leave Gender and Address fields empty
3. Fill the remaining fields with valid data
4. Click on "Submit"

### Expected Result
- Employee should not be registered
- Validation error message should be displayed for both missing fields

### Actual Result
- The system allows to leave Gender and Address field empty
- Employee registration is completed succesfully

### Status
Open

---

## 🐞 BG007 - System allows addresses and phone numbers shorter than the established minimum

### Environment
Windows 10, Google Chrome (Version 147.0.7727.56)

### Priority
High

### Severity
High

### Description
The Address and Phone fields can be filled with data shorter than the established minimum

### Steps to Reproduce
1. Open Employee Registration form
2. Enter short address (e.g., 3 characters)
3. Enter short phone number (e.g., 5 characters)
4. Fill the remaining fields with valid data
5. Click on "Submit"

### Expected Redult
- The system should not accept addresses or phone numbers shorter than 10 characters (established minimum)
- Validation error mesage should be displayed in both fields indicating requirements

### Actual Result
- Employees can be registered with addresses and phone numbers with fewer characters than the established minimum

### Status
Open

---

## 🐞 BG008 - Employee Registration table exceeds the form limits

### Environment
Windows 10, Google Chrome (Version 147.0.7727.56)

### Priority
Medium

### Severity
Medium

### Description
The Employee Registration table at the bottom of the form exceeds its limits

### Steps to Reproduce
1. Open Employee Registration form
2. Fill every field with valid data
3. Click on "Submit"
4. View the registration table displayed under the form

### Expected Result
- The registration table should adjust to the form's size

### Actual Result
- The registration table expands outside the form's boundaries

### Status
Open
