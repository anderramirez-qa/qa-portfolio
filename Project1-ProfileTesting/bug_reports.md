## Project: Buggy Cars Testing

# 🐞 Bug Reports - Buggy Cars
Application: https://buggy.justtestit.org/

---

## 🐞 BG001 — Incorrect validation message for Last Name field on Registration page

### Environment
Windows 10, Chrome

### Priority
Medium

### Severity
Minor

### Description
The validation message for the Last Name field is incorrect. It displays “First Name is required” instead of “Last Name is required”.

### Steps to Reproduce
1. Navigate to https://buggy.justtestit.org/  
2. Click on "Register"  
3. Leave Last Name field empty  
4. Submit the form  

### Expected Result
Validation message should display: “Last Name is required”

### Actual Result
Validation message displays: “First Name is required”

### Status
Open

---

## 🐞 BG002 — Unclear and technical validation message for password field

### Environment
Windows 10, Chrome

### Priority
Medium

### Severity
Minor

### Description
Password validation message contains technical terms that are not user-friendly and may confuse users.

### Steps to Reproduce
1. Navigate to https://buggy.justtestit.org/register  
2. Enter password with less than 6 characters  
3. Submit form  

### Expected Result
Clear message such as: “Password must contain at least 6 characters”

### Actual Result
Message displays: “Invalid parameter SignUpInput.password”

### Status
Open

---

## 🐞 BG003 — Navigation link "Buggy Rating" does not redirect to Home page

### Environment
Windows 10, Chrome

### Priority
High

### Severity
Major

### Description
The "Buggy Rating" navigation link does not redirect to the home page when clicked.

### Steps to Reproduce
1. Navigate to https://buggy.justtestit.org/  
2. Click on "Popular Make"  
3. Click on "Buggy Rating"  

### Expected Result
User should be redirected to home page

### Actual Result
No action occurs

### Status
Open

---

## 🐞 BG004 — Broken image for "Lancia Ypsilon" on Overall Rating page

### Environment
Windows 10, Chrome

### Priority
Low

### Severity
Minor

### Description
Image for "Lancia Ypsilon" is not displayed.

### Steps to Reproduce
1. Navigate to Overall Rating page  
2. Go to page 4  
3. Locate "Lancia Ypsilon"  

### Expected Result
Car image should be displayed

### Actual Result
Image is broken / not displayed

### Status
Open

---

## 🐞 BG005 — Sorting by Rank displays incorrect order

### Environment
Windows 10, Chrome

### Priority
High

### Severity
Major

### Description
Sorting by Rank does not display results in correct numerical order.

### Steps to Reproduce
1. Navigate to Overall Rating page  
2. Click on "Rank" column  

### Expected Result
List should be sorted numerically (ascending/descending)

### Actual Result
Incorrect order is displayed

### Status
Open

---

## 🐞 BG006 — Sorting by Votes is not working

### Environment
Windows 10, Chrome

### Priority
High

### Severity
Major

### Description
Sorting functionality for "Votes" column does not work.

### Steps to Reproduce
1. Navigate to Overall Rating page  
2. Click on "Votes" column  

### Expected Result
List should be sorted by number of votes

### Actual Result
No sorting occurs

### Status
Open

---

## 🐞 BG007 — Pagination allows navigation beyond last page

### Environment
Windows 10, Chrome

### Priority
Medium

### Severity
Major

### Description
User can navigate beyond available pages.

### Steps to Reproduce
1. Navigate to Overall Rating page  
2. Go to last page  
3. Click "Next" repeatedly  

### Expected Result
Navigation should stop at last page

### Actual Result
User can access non-existing pages

### Status
Open

---

## 🐞 BG008 — Popular Model page not responsive on mobile

### Environment
Mobile (Chrome)

### Priority
High

### Severity
Critical

### Description
Page becomes unresponsive and keeps loading due to long comments.

### Steps to Reproduce
1. Open site on mobile  
2. Navigate to "Popular Model"  

### Expected Result
Page should load and display content correctly

### Actual Result
Page keeps loading indefinitely

### Status
Open

---

## 🐞 BG009 — Comment authors are not displayed

### Environment
Windows 10, Chrome

### Priority
Medium

### Severity
Minor

### Description
Comments are displayed without showing author names.

### Steps to Reproduce
1. Navigate to model page  
2. Scroll to comments section  

### Expected Result
Author names should be visible

### Actual Result
Author names are missing

### Status
Open

---

## 🐞 BG010 — Profile allows saving empty values (spaces only)

### Environment
Windows 10, Chrome

### Priority
High

### Severity
Major

### Description
System allows saving first name and last name with only spaces.

### Steps to Reproduce
1. Navigate to Profile  
2. Enter spaces in name fields  
3. Click Save  

### Expected Result
System should reject empty/invalid values

### Actual Result
System accepts invalid input

### Status
Open

---

## 🐞 BG011 — Gender field allows invalid values and throws error

### Environment
Windows 10, Chrome

### Priority
Medium

### Severity
Major

### Description
User can enter invalid values in Gender field leading to system error.

### Steps to Reproduce
1. Navigate to Profile  
2. Enter custom value in Gender  
3. Click Save  

### Expected Result
Only predefined values should be accepted

### Actual Result
System throws "unknown error"

### Status
Open

---

## 🐞 BG012 — Phone field accepts invalid characters

### Environment
Windows 10, Chrome

### Priority
Medium

### Severity
Major

### Description
Phone field accepts special characters.

### Steps to Reproduce
1. Navigate to Profile  
2. Enter special characters (e.g., +++++ )  
3. Click Save  

### Expected Result
Only numeric values should be accepted

### Actual Result
Invalid data is accepted

### Status
Open
