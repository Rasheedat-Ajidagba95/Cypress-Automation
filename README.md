# Cypress-Automation

# 🛒 E-Commerce Test Automation with Cypress

This project contains automated test scripts for the e-commerce website [AskOmDch](https://askomdch.com/), written using [Cypress](https://www.cypress.io/). It covers essential user flows such as signup, login, product search, product filter, product sorting, add to cart, checkout,and order management.

---

## 📌 Project Overview

This test suite is designed to:

- Verify key functionalities of the AskOmDch online store
- Validate end-to-end user flows
- Improve confidence in releases by catching bugs early

Automation is implemented using Cypress (JavaScript-based end-to-end testing framework) for fast, reliable, and readable tests.

---

## 🧪 Features Tested

- User SignUp
- User Login
- Product Search
- Product Filter
- Product Sorting
- Add to Cart
- View Cart
- Checkout Process
- View order list
- View order Individual Details
- UI Element Visibility
- Assertions on Page Titles and Text
- Negative Testing for Invalid Inputs

---

## ⚙️ Tech Stack

- **Framework:** Cypress
- **Language:** JavaScript
- **Test Runner:** Cypress UI and CLI

---

##  Getting Started

### Prerequisites

- Node.js installed (v14+ recommended)
- Git installed
- Package manager (npm or yarn)

### Installation

1. Clone the repo:

*bash*
git clone git@github.com:Rasheedat-Ajidagba
cd Cypress-Automation


2. Install dependencies:
*bash*
npm init


3. Open Cypress Test Runner:

*bash*
npx cypress open


Or run tests in headless mode:

*bash*
npx cypress run


---

## 📂 Folder Structure


cypress/
│
├── e2e/                                      # Test specs
│   └── authentication.spec.cy.js             # Signup and Login tests
│   └── cartAndCheckout.spec.cy.js            # Add to cart & checkout
│   └── filterProductByCategories.spec.cy.js  # Filter products by different categories
│   └── orderManagement.spec.cy.js            # Check order lists and view order details
│   └── searchProduct.spec.cy.js              # Search for products
|   └── sortProducts.spec.cy.js               # Sort products 
│
|
├── fixtures/                                # Test data
│   └── element.json
│
├── support/               
│   └── commands.js                         # Custom Cypress commands
│   └── e2e.js             # Global config
│
cypress.config.js          # Cypress config file


---

## 🧾 Sample Command

Example of a custom command used in the tests:

*javascript*
Cypress.Commands.add('successfullLogin', () => {
  cy.get(login.emailField).should('be.visible').type("email");
    cy.get(login.passwordField).should('be.visible').type("password");
    cy.get(login.loginButton).should('be.visible').click();
})
```

---

## 🧠 Author

**Rasheedat Ajidagba** 
QA Engineer | Test Automation Enthusiast  

---

## ✅ Status

Project is actively maintained and can be extended to include more test scenarios such as:

- Payment integration testing
- Responsive layout testing

---


