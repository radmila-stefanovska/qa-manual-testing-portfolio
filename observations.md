# Exploratory Testing Observations

## Observation 001

Module: Login

Scenario:
Valid username + empty password

Expected:
Only the Password field should be highlighted.

Actual:
Both Username and Password fields are highlighted.

Status:
Needs clarification with design specification.

---

## Observation 002

Module:
Products

User:
problem_user

Scenario:
Verify product images on the Products page.

Expected Result:
Each product should display its corresponding product image.

Actual Result:
All products display the same dog image (dog holding a tennis ball) instead of their corresponding product images.

Status:
Expected behavior for the problem_user test account / exploratory observation.

Notes:
Behavior should be verified using standard_user before reporting as a defect.
---

## Observation 003

Module: Performance

User:
performance_glitch_user

Scenario:
Navigation between pages

Actual:
Each page loads in approximately 7 seconds.

Status:
Expected behavior for performance test user.

## Observation 004

Module:
Login

User:
standard_user

Scenario:
Valid username + wrong password

Expected Result:
Only the Password field should be highlighted because the username is valid and the password is incorrect.

Actual Result:
Both Username and Password fields are highlighted in red, even though the Username value is valid.

Status:
Potential UI/UX issue / needs clarification with design specification.

Notes:
Error message correctly prevents login, but field-level validation may be misleading for the user.

OBS-005

Module:
Checkout

Scenario:
Checkout with an empty shopping cart.

Observation:
The application allows users to complete the checkout process even when no products are present in the shopping cart.

Expected Behavior:
Unable to determine without business requirements.

Recommendation:
Verify expected checkout flow with Product Owner or functional specification before reporting as a defect.
