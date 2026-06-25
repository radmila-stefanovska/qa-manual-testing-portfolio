# Bug Reports

This document contains defects identified during exploratory testing of the SauceDemo web application.

---

# BUG-001

## Title

Product prices change after returning from the Product Details page

## Module

Products

## Environment

- Browser: Google Chrome
- Operating System: Windows 11
- Test User: visual_user

## Severity

High

## Priority

High

## Preconditions

- User is logged in as `visual_user`.

## Steps to Reproduce

1. Login as `visual_user`.
2. Observe product prices on the Products page.
3. Open any product.
4. Verify the product price on the Product Details page.
5. Click **Back to Products**.
6. Compare the prices on the Products page.

## Expected Result

Product prices should remain consistent before and after opening a product.

## Actual Result

After returning to the Products page, product prices change and no longer match the original prices.

## Reproducibility

100%

## Status

Open

## Attachments

- screenshots/bug-001-products-before.png
- screenshots/bug-001-product-details.png
- screenshots/bug-001-products-after.png

---

# BUG-002

## Title

Checkout can be completed with an empty shopping cart

## Module

Checkout

## Environment

- Browser: Google Chrome
- Operating System: Windows 11
- Test User: standard_user

## Severity

Medium

## Priority

Medium

## Preconditions

- User is logged in.
- Shopping cart is empty.

## Steps to Reproduce

1. Login as `standard_user`.
2. Open the shopping cart without adding any products.
3. Click **Checkout**.
4. Enter First Name, Last Name and Zip Code.
5. Click **Continue**.
6. Click **Finish**.

## Expected Result

The application should prevent checkout completion when no products are present in the shopping cart.

## Actual Result

The checkout process completes successfully and displays the message:

> Thank you for your order!

## Reproducibility

100%

## Status

Open

## Note

This defect is reported based on expected e-commerce checkout behavior. The expected behavior should be confirmed against business requirements.

## Attachments

- screenshots/bug-002-empty-cart.png
- screenshots/bug-002-order-complete.png
