# Login Test Cases

Application Under Test:
https://www.saucedemo.com/

---

## TC-001 Valid Login

Priority: High

Preconditions:
- User is on the login page.
- User has valid credentials.

Test Steps:

1. Open https://www.saucedemo.com/
2. Enter username: standard_user
3. Enter password: secret_sauce
4. Click Login

Expected Result:

- User is redirected to the Products page.
- Inventory list is displayed successfully.

---

## TC-002 Invalid Password

Priority: High

Preconditions:
- User is on the login page.

Test Steps:

1. Open https://www.saucedemo.com/
2. Enter username: standard_user
3. Enter password: wrong_password
4. Click Login

Expected Result:

- User remains on the login page.
- Error message is displayed.

---

## TC-003 Empty Username

Priority: Medium

Test Steps:

1. Open login page.
2. Leave Username empty.
3. Enter password: secret_sauce
4. Click Login

Expected Result:

Error message:
"Username is required"

---

## TC-004 Empty Password

Priority: Medium

Test Steps:

1. Open login page.
2. Enter username: standard_user
3. Leave Password empty
4. Click Login

Expected Result:

Error message:
"Password is required"
