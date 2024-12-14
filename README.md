# Validation-Form-React
This project demonstrates form validation in React using [Formik] and [Yup] for managing form state and validating user inputs. It includes features such as email validation, password strength indicators, and more.

## Table of Contents
1. [How to Run the Project](#how-to-run-the-project)
2. [Features](#features)
3. [Design Choices](#design-choices)
4. [Assumptions and Limitations](#assumptions-and-limitations)


## How to Run the Project


### 1. Install Dependencies

Make sure you have Node.js installed. Then, install the required dependencies by running:

```bash
npm install
```

Alternatively, if you're using Yarn:

```bash
yarn install
```

### 2. Run the App

To run the app in your local development environment:

```bash
npm start
```

This will start a local development server, and you can view the app by visiting `http://localhost:3000` in your browser.

---

## Features

- Sign Up & Login Forms: Forms are built using Formik, allowing easy state management and validation.
- Email Validation: The app validates the email input field to ensure it's in a correct format.
- Password Validation: The app enforces a minimum length requirement for passwords and provides a Password Strength Meter.
- Error Handling: Clear error messages are displayed for invalid inputs.
- "Remember Me": The app includes a "Remember Me" checkbox for login, storing user email in localStorage.


## Design Choices

### 1. Form Handling with Formik

Formik is used to handle form state and validation. Formik’s API allows for easy management of complex forms, making it a perfect fit for React applications with dynamic form inputs.

### 2. Validation with Yup

Yup is used for validation. This library provides a schema-based validation approach and works seamlessly with Formik, allowing us to define a validation schema that applies to the entire form or individual fields.

Example validation schemas include:
- Email: Must follow a standard email format.
- Password: Must have a minimum length of 8 characters.

### 3. Password Strength Meter

For the Sign Up form, a password strength meter provides users with real-time feedback on how strong their chosen password is. This encourages users to create stronger, more secure passwords.

### 4. UI Design

The UI of this app is simple and minimalist, making it easy to navigate. It focuses on usability with clearly labeled form inputs and error messages.

### 5. Accessibility

The app is designed with accessibility in mind:
- Input fields have clear labels.
- Error messages are displayed beneath the corresponding form field, helping users with disabilities understand what went wrong.

---

## Assumptions and Limitations

### Assumptions:

- Email Validation: The app assumes users will enter a valid email address, which is validated using the Yup library.
- Password Strength: The app uses basic password validation (minimum length of 8 characters). More advanced validation (including special characters, uppercase letters, etc.) could be added for stronger security.

### Limitations:

- No Backend Integration: This is a frontend-only app for demonstration purposes. It doesn't interact with a backend to authenticate users or store form data.
- Basic Password Strength Meter: The current password strength indicator is based purely on the length of the password. It doesn't check for the presence of uppercase letters, numbers, or special characters, which are common in production-level password strength indicators.
- Basic Authentication: No actual login or signup logic has been implemented. This would require integration with an API or backend server to store and validate user credentials.
- Limited Error Handling: While validation errors are shown, there's no sophisticated error handling for edge cases (e.g., server-side validation, network errors).

---



## Technologies Used

- React: The front-end library used to build the user interface.
- Formik: A form library for managing form state and validation.
- Yup: A schema builder for validating values.
- CSS/SCSS: For styling the app.
- LocalStorage: For storing user data (e.g., email) in the browser for the **Remember Me** functionality.


