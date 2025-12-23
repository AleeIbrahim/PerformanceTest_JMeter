# JMeter Test Plan: JPetStore Purchase Workflow

## Overview
This JMeter test plan simulates the end-to-end purchase workflow for the JPetStore demo application. It is designed to validate the performance and functionality of the online shopping process under load.

## Test Scenarios
The plan includes 5 independent user groups (User 1–2, User 3–4, etc.), each performing the following steps:

1. **Login Setup** – CSV Data Set Config for user credentials
2. **Home Page** – Access JPetStore Home Page
3. **Browse Category** – Navigate to Fish Category
4. **Product Selection** – Choose a specific product
5. **Shopping Cart** – Add selected product to cart
6. **Checkout** – Proceed to checkout and navigate to Login Page
7. **Payment Process** – Confirm and submit payment details (repeated for validation)
8. **Completion** – Return to Main Menu

Each user group includes a **Constant Timer** to control pacing between iterations.

## Purpose
- Validate the purchase flow under simulated user load; where the load is gradually increased by 2 users each 3 minutes, till it reaches 10 concurrent users.
- Measure response times for common user actions.

## Notes
- Uses CSV-based login data for parameterization.
- Modular structure allows easy scaling of virtual users.
- Timers are included to simulate realistic think time between steps.

