# JMeter Test Plan: JPetStore Purchase Workflow

## Overview
This JMeter test plan simulates the end-to-end purchase workflow for the JPetStore demo application. It is designed to validate the performance and functionality of the online shopping process under load.

## Test Scenarios
The plan includes two independent user groups (User 1–2 and User 3–4), each performing the following steps:

1. **Login Setup** – CSV Data Set Config for user credentials
2. **Home Page** – Access JPetStore Home Page
3. **Browse Category** – Navigate to Fish Category
4. **Product Selection** – Choose a specific product
5. **Shopping Cart** – Add selected product to cart
6. **Checkout** – Proceed to checkout and navigate to Login Page
7. **Payment Process** – Confirm and submit payment details (repeated for validation)
8. **Completion** – Return to Main Menu

Each user group includes a **Constant Timer** to control pacing between iterations.

## Files Included
- `image.png` – Screenshot of the JMeter test plan structure

## Purpose
- Validate the purchase flow under simulated user load.
- Ensure correct data handling via CSV login sets.
- Measure response times for critical user actions.

## Notes
- Uses CSV-based login data for parameterization.
- Modular structure allows easy scaling of virtual users.
- Timers are included to simulate realistic think time between steps.

