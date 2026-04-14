# Mobile Data Collection API

## Overview
This API supports a mobile application used by field consultants to collect and manage farmer data across FPOs. It enables real-time data capture and retrieval.

---

## Base URL
https://api.farmerdata.app/v1

---

## Authentication
All requests require a Bearer Token in the header:

Authorization: Bearer <access_token>

---

## Endpoints

The API documentation includes the following endpoints to demonstrate structured and complete technical documentation:

### 1. Submit Farmer Data (POST `/collect-data`)
- Captures farmer data collected by field consultants  
- Includes structured request body and success response  

### 2. Fetch Farmer Records (GET `/farmer-records`)
- Retrieves farmer records based on query parameters  
- Demonstrates filtering and structured response handling  

### 3. Update Farmer Record (PUT `/update-record/{record_id}`)
- Updates existing farmer data  
- Includes request body and confirmation response  

### Error Handling
- Standardized error response structure  
- Includes common HTTP status codes (400, 401, 404, 500)

---

## Documentation Samples

- [API Documentation – Mobile Data Collection App](./api-docs.md)  
- [User Guide – Mobile Data Collection App](./user-guide.md)  
- [Editing and Clarity Improvement Sample](./editing-sample.md)  
- [Documentation Style Guide](./style-guide.md)

---

## Audience and Context

- **API Documentation** → Intended for developers integrating and maintaining backend services  
- **User Guide** → Designed for field consultants with limited technical background  
- **Editing Sample** → Demonstrates clarity improvement and ambiguity resolution  
- **Style Guide** → Demonstrates approach to maintaining consistency in documentation  

---

## Editorial Approach

The documentation samples focus on:

- Improving clarity without altering technical intent  
- Structuring information for usability and readability  
- Resolving ambiguous or unclear technical statements  
- Maintaining consistency across documents  

---

## Note

All samples are based on prior project experience and are anonymized for demonstration purposes.
