## Project: Buggy Cars Testing

# 🧪 Profile Testing - Test Cases

---

## TC_PROFILE_001 — Update user profile with valid data

### Feature
User Profile Management

### Priority
High

### Severity
Critical

### Preconditions
- User is registered
- User is logged into the system
- User is on the Profile page

### Test Data
- First Name: Juan
- Last Name: Pérez
- Address: Calle Mayor 123
- Phone: 600123456
- Hobby: Football
- Password: ValidPass@123

### Steps to Reproduce
1. Open browser
2. Navigate to https://buggy.justtestit.org/
3. Log in with valid credentials
4. Click on "Profile"
5. Enter valid data in all editable fields
6. Click on "Save"

### Expected Result
- User profile is updated successfully
- Success confirmation message is displayed
- Updated data is visible after reload

### Actual Result
User profile updated successfully

### Status
PASS

---

## TC_PROFILE_002 — Attempt to update user profile without making any changes

### Feature
User Profile Management

### Priority
Medium

### Severity
Medium

### Preconditions
- User is registered
- User is logged into the system
- User is on the Profile page

### Test Data
- First Name: Juan
- Last Name: Pérez
- Address: Calle Mayor 123
- Phone: 600123456
- Hobby: Football
- Password: ValidPass@123

### Steps to Reproduce
1. Open browser
2. Navigate to https://buggy.justtestit.org/
3. Log in with valid credentials
4. Click on "Profile"
5. Click on "Save"

### Expected Result
- System should not update the profile
- No changes should be saved
- System should display a message indicating no changes
- Save should be disabled OR no confirmation shown

### Actual Result
User profile updated successfully

### Status
FAIL

---

## TC_PROFILE_003 — Attempt to update profile with password missing uppercase letter

### Feature
User Profile Management

### Priority
High

### Severity
High

### Preconditions
- User is registered
- User is logged into the system
- User is on the Profile page

### Test Data
- Password: validpass@123

### Steps to Reproduce
1. Open browser
2. Navigate to https://buggy.justtestit.org/
3. Log in with valid credentials
4. Click on "Profile"
5. Enter password without uppercase letters
6. Click on "Save"

### Expected Result
- Profile should not be updated
- Validation error message should be displayed
- Error should indicate missing uppercase requirement

### Actual Result
- Profile is not updated
- Validation error message is displayed

### Status
PASS

---

## TC_PROFILE_004 — Attempt to update profile with valid password of exactly 6 characters (boundary testing)

### Feature
User Profile Management

### Priority
High

### Severity
High

### Preconditions
- User is registered
- User is logged into the system
- User is on the Profile page

### Test Data
- Password: Vp@ss1

### Steps to Reproduce
1. Open browser
2. Navigate to https://buggy.justtestit.org/
3. Log in with valid credentials
4. Click on "Profile"
5. Enter password with exactly 6 characters
6. Click on "Save"

### Expected Result
- Profile should be updated successfully
- Success message should be displayed
- Password should be accepted

### Actual Result
- Profile is not updated
- Validation error message is displayed

### Status
FAIL
