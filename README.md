# Secure Login Application

## Overview

This application has been remediated to address several security vulnerabilities following the OWASP Top Ten guidelines.

### Remediations

1. **Insecure Storage in `localStorage`**: Removed usage of `localStorage` for storing credentials.
2. **Insecure Password Management**: Implemented server-side authentication to handle credentials securely.
3. **Cross-Site Scripting (XSS)**: Sanitized user input using DOMPurify to prevent XSS attacks.
4. **HTTPS Enforcement**: Ensure the application uses HTTPS for secure communication.

Each remediation has been committed on its respective feature branch and merged into the main branch following best practices.

## Git Workflow

The development process involved the following steps:

1. Creation of the `develop` branch from `main`.
2. Creation of individual feature branches for each remediation.
3. Merging each feature branch back into `develop`.
4. Final merge of `develop` into `main`.

This workflow ensures that each change is isolated and can be reviewed independently.

## Setup

To run this application, ensure your server is configured to enforce HTTPS and handle POST requests securely.

1. Clone the repository:
   ```sh
   git clone <repository-url>
   cd secure-login

