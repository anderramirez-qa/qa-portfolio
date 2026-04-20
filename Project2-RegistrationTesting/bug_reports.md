## Project: GeekRetail Registration Testing

# 🐞 Bug Reports - GeekRetail
Test form: https://testing1.geekqa.net/

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
4. Click on "submit"

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

### Enviroment
Windows 10, Google Chrome (Version 147.0.7727.56)

### Priority
Medium

### Severity
Medium

### Description
System accepts values outside the established range (18-65) in the Age field

### Steps to Reproduce
1. Open Employee Registration form
2. Enter "5" in the Age field
3. Fill the remaining fields with valid data
4. Click on "submit"

### Expected Result
- System should displayed an error message indicating age should be within the established range
- Employee registration failed

### Actual Result
- System accepts invalid Age data and employee is registered succesfully

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
5. Click on "submit"

### Expected Result
- Validation error message should be displayed indicating inconsistent data between Age and Date of Birth fields
- System should not allow registration

### Actual Result
- System accepts different values for Age and Date of Birth fields
- Employee is registered and added to the table

### Status
Open

---

## 🐞 BG004 - Expected Salary column always displays "0"

### Environment
Windows 10, Google Chrome (Version 147.0.7727.56)

### Priority
High

### Severity
Critical

### Description
The Expected Salary column always displays "0" regardless of the value entered in the field

### Steps to Reproduce
1. Open Employee Registration form
2. Enter any valid data in the Expected Salary field (e.g., 30000)
3. Fill the remaining fields with valid data
4. Click on "submit"

### Expected Result
- Employee registration should be successfull and displayed correctly on the table
- Expected Salary column should displayed the entered data

### Actual Result
- Expected Salary column always displays "0" regardless of the data entered in the field

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
4. Click on "submit"

### Expected Result
- The system should not allow the selection of any future or non-existent dates

### Actual Result
- Systems accepts any date, past and future, in the Date of Birth field
- Registration is completed successfully

### Status
Open

---

## 🐞 BG006 - 
