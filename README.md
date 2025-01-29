# API Test Automation with Bruno

[![API Test Automation with Bruno](https://github.com/testsmith-io/api-test-automation-bruno/actions/workflows/bruno.yml/badge.svg)](https://github.com/testsmith-io/api-test-automation-bruno/actions/workflows/bruno.yml)

This repository contains example collections and scripts for API test automation using:
- **Bruno** for API request management and testing.
- **Bruno CLI** for running Bruno collections via the command line.

## Features
- Examples of GET, POST, and Protected API requests.
- Comprehensive demonstration of API testing workflows with assertions and pre/post-request scripts.
- Fully automated CI pipeline using GitHub Actions to run Bruno collections.

## Test API
All examples in this repository are designed to work with the **Practice Software Testing API**, a publicly available API for learning and practicing software testing. You can explore the API documentation and endpoints here:  
👉 **[Practice Software Testing API](https://api.practicesoftwaretesting.com/api/documentation)** 👈

## Examples Included
1. **GET Request**: Fetch a list of brands with `GET /brands`.
2. **Login API**: Authenticate using `POST /login` with an email/password payload.
3. **Protected API Request**: Authenticate, then use a token to fetch data with `GET /invoices`.

## Prerequisites
- **Bruno** installed locally.
- **Bruno CLI**, the Bruno command-line tool. Install it globally with:
  ```bash
  npm install -g @usebruno/cli
  ```

## Setup and Run
1. Clone this repository:
   ```bash
   git clone https://github.com/testsmith-io/api-test-automation-bruno.git
   ```
2. Navigate to the project directory:
   ```bash
   cd api-test-automation-bruno
   ```
3. Run the Bruno collection using Newman:
   ```bash
   bru run --env test --reporter-html results.html
   ```

## Automated Workflow
The repository includes a GitHub Actions workflow to automatically execute the Bruno collections with Newman. It runs on every `push` and `pull_request` to ensure the tests pass seamlessly.