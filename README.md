# Forms and Validation Assignment

**Name:** Alish Medina  
**Group:** SE-2538

---

## Overview
This project demonstrates HTML form building and validation using **Bootstrap 5.3**. It contains five tasks, each focusing on a different aspect of form design and validation - from basic inputs to advanced JavaScript-based validation.

---

## Task 0: Simple Contact Form
A basic contact form with Name, Email, Message, and Submit button. All fields have proper `<label>` elements. No validation - this is the plain baseline.

<img width="1323" height="671" alt="Снимок экрана 2026-10-13 173225" src="https://github.com/user-attachments/assets/0e4130d8-c9a2-4c65-977e-887a734a58b2" />

---

## Task 1: HTML5 Validation
Same form structure as Task 0, but with built-in HTML5 validation attributes:
- `required` on all fields
- `type="email"` on email
- `maxlength="30"` on name
- `maxlength="200"` on message
The browser blocks submission and shows native error popups for invalid inputs.

<img width="1202" height="548" alt="Снимок экрана 2026-10-13 173214" src="https://github.com/user-attachments/assets/6e57ad99-d50b-4267-a61e-33c3ee78248c" />

---

## Task 2: Bootstrap Contact Form
Recreated the contact form using Bootstrap classes:
- Bootstrap grid (`row`, `col-md-6`) for responsive layout
- `form-control`, `form-label`, `form-text` classes
- Placeholders for all fields
- Helper text ("We'll never share your email.")

<img width="1167" height="623" alt="Снимок экрана 2026-10-13 173248" src="https://github.com/user-attachments/assets/28127431-55b4-49d6-8ebd-3f76a3746265" />

---

## Task 3: Bootstrap Validation
Demonstrates Bootstrap's validation feedback system:
- `novalidate` disables the browser's default popups
- JavaScript adds the `was-validated` class on submit
- `invalid-feedback` and `valid-feedback` show red/green messages

<img width="1100" height="465" alt="Снимок экрана 2026-10-13 174308" src="https://github.com/user-attachments/assets/f2dead43-8f0c-4130-a612-579ae63574f7" />

---

## Task 4: Registration Form
A complete registration form combining everything:
- First Name, Last Name, Email
- Password + Confirm Password (must match)
- Gender radio buttons
- Hobbies checkboxes
- Country dropdown
- Submit and Reset buttons

**Validation features:**
- Bootstrap grid for responsive layout
- HTML5 `minlength="8"` on password
- Custom JavaScript for password matching (`setCustomValidity`)
- Custom gender selection check
- Bootstrap validation feedback on all fields
- Success message on valid submission

<img width="1096" height="825" alt="Снимок экрана 2026-10-13 173422" src="https://github.com/user-attachments/assets/3143ef61-44f3-405f-a9fb-57ac10740939" />
<img width="1126" height="820" alt="Снимок экрана 2026-10-13 173500" src="https://github.com/user-attachments/assets/52a380d2-60f1-4e9d-ba5d-bfe415d44920" />

---

## Summary
I built five forms, each demonstrating a different part of HTML form building - from basic inputs to Bootstrap validation. The most interesting parts were:
1. **Understanding the difference between HTML5 validation and Bootstrap validation** - HTML5 shows browser popups, while Bootstrap shows inline red/green borders and messages.
2. **Password matching with `setCustomValidity`** - since HTML5 has no built-in "passwords must match" rule, this had to be done in JavaScript.
3. **Radio button group validation** - Bootstrap's feedback system works on single inputs, so I checked the radio group manually with `document.querySelector('input[name="gender"]:checked')`.

All forms are responsive, styled consistently, and validate correctly.

---

## How to Run
1. Clone the repository
2. Open `index.html` in any modern browser
3. No installation or build step needed - Bootstrap loads from CDN

---

## Files
- `index.html` - all five forms
- `style.css` - custom styling
- `screenshots/` - screenshots for each task
