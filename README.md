# Online-Banking-QA-Project
This project simulates manual testing of a small online banking web application that supports secure login, balance viewing, fund transfers, and transaction history. It demonstrates functional testing, negative testing, usability testing, boundary analysis, and risk-based testing.

**1. Application Features (Defined Requirements)**

**User Authentication**

R1.1: Users must log in using a valid username and password.

R1.2: Invalid credentials should show an error message.

R1.3: System locks the account after 5 failed attempts.

**Account Dashboard**

R2.1: User can view their current balance.

R2.2: User can view latest 10 transactions.

**Funds Transfer**

R3.1: User can transfer funds to another internal account.

R3.2: Transfer requires amount, recipient account number, and description.

R3.3: Amount must be between $1 and $5,000.

R3.4: System must show confirmation before processing.

**Transaction History**

R4.1: User can view complete history with date, type, and amount.

R4.2: User can filter by date range.

Security & Session Management

R5.1: Session expires after 10 minutes of inactivity.

R5.2: User is logged out on browser close.

**2.Test Plan Summary Scope**

This project covers functional, usability, security-adjacent (non-penetration), and compatibility testing for the banking application.

Out of Scope

Automation

Performance & load testing

Penetration testing

Backend database integrity beyond visible data

Test Types

Functional Testing

UI/UX Testing

Negative Testing

Boundary Value Analysis

Risk-Based Testing

Regression Testing

Test Environment

OS: Windows/macOS

Browsers: Chrome, Firefox, Edge

Test Data: Dummy customer accounts (non‑real data)

**3.Test Scenarios**
**Login & Authentication**

Verify login with valid credentials.

Verify login failure with invalid username.

Verify login failure with invalid password.

Verify account lockout after 5 failed attempts.

Verify successful logout.

**Dashboard**

Verify balance displays correctly.

Verify last 10 transactions display.

Funds Transfer

Verify successful transfer with valid details.

Verify error on insufficient balance.

Verify boundary values: $0, $1, $5,000, $5,001.

Verify transfer fails with invalid target account.

Verify user sees confirmation modal.

**Transaction History**

Verify full list loads.

Verify date filter returns correct results.

Verify empty results message when no transactions match.

**Session & Security**

Verify session timeout after 10 min.

Verify logout on browser close.

Verify user cannot navigate back after logout.


