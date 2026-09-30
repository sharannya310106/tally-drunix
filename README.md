# Tally: One Agreed Truth for Every Stuck Payment

**Status:** Proposal Stage
**Event:** DRUNIX Hackathon 2026 — In collaboration with Citi
**Problem Statement:** Real-Time Payments

## Problem Statement

Real-time digital payments may encounter network interruptions, delayed responses, or communication failures. In such situations, the payer, payee, and payment service provider may have different views of the same transaction.

For example, a payment may time out even though the payer's account has been debited, leaving the final transaction status uncertain. Retrying without checking the status may create duplicate-payment risks, while manual reconciliation can require additional time and effort.

## Proposed Solution

Tally is a proposed payment accountability and reconciliation platform designed to help participating institutions track transaction events and resolve uncertain payment outcomes.

The system aims to maintain a shared, auditable record of payment-status reports, identify conflicting information, enforce defined resolution deadlines, and track the progress of unresolved transactions.

Duplicate reports will be handled idempotently, and transaction-state changes will follow defined business rules.

## Key Features

* **Shared transaction history:** Maintain a traceable record of transaction events.
* **Conflict detection:** Identify inconsistent transaction-status reports.
* **Resolution tracking:** Track unresolved payments and configurable deadlines.
* **Duplicate protection:** Detect repeated requests using idempotency mechanisms.
* **Audit trail:** Record transaction-state changes and resolution actions.
* **Scenario simulator:** Demonstrate timeouts, delayed confirmations, duplicate requests, and conflicting reports.

## Planned Architecture

* **DRUNIX:** Intended platform for the core transaction workflow, subject to verification of available capabilities.
* **Smart business logic:** Planned transaction lifecycle and conflict-resolution rules, implemented using the mechanisms supported by DRUNIX.
* **Backend:** Node.js and Express.js.
* **Frontend:** React.js with Vite.
* **Database:** MongoDB for application records and dashboard read models.
* **Testing:** Simulated institutions and payment events for controlled testing.

## Implementation Roadmap

* [ ] Review DRUNIX documentation and developer resources.
* [ ] Identify the supported platform integration and testing environment.
* [ ] Design transaction states and reconciliation rules.
* [ ] Implement the core transaction workflow.
* [ ] Develop the backend API and simulated institution adapters.
* [ ] Build the transaction monitoring dashboard.
* [ ] Test timeouts, duplicate requests, conflicting reports, and delayed confirmations.
* [ ] Document the architecture, setup instructions, test results, and demo.

## Security and Testing

The prototype will use simulated institutions and test transactions. It will not transfer real money or require real customer banking data.

Authentication, role-based access controls, input validation, and secure handling of credentials will be considered during implementation.

## Expected Impact

Tally aims to improve transaction visibility, reduce unnecessary duplicate payment attempts, and simplify the resolution of uncertain payment outcomes.

The prototype will be evaluated using transaction-status accuracy, duplicate-request handling, reconciliation time, and the successful resolution of test scenarios.

## Repository Status

This repository currently contains the project proposal and development roadmap. Implementation details and test results will be added as development progresses.

## Team

* Sharannya Jadhav
* Add other team members, if applicable
