# Demo API Testing - Postman

## Overview

API automation project created using Postman and Postman CLI.

## API

Restful Booker API

## Test Scenarios

- Authentication and token extraction
- Create booking
- Get booking by ID
- Search booking by first name
- Update booking using PATCH
- Delete booking
- Response status code validation
- Response body validation
- Content-Type validation
- Response time validation
- Dynamic environment variables

## Automation Flow

POST /auth
   ↓
Extract authentication token
   ↓
POST /booking
   ↓
Extract booking ID
   ↓
GET booking
   ↓
PATCH booking
   ↓
Verify updated data
   ↓
DELETE booking

## Execution

The collection can be executed locally using Postman CLI:

postman collection run ./postman/Demo_API_Test.postman_collection.json --environment ./postman/QA_Envi_Demo.postman_environment.json

## Test Result

- Requests: 6
- Assertions: 17
- Passed: 17
- Failed: 0

## CI/CD

GitHub Actions CI/CD will be added in the next phase.
