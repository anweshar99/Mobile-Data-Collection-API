# Mobile Data Collection API

## Overview
This API supports a mobile application (see [User Guide](./user-guide.md)) used by field consultants to collect and manage farmer data across FPOs. It enables real-time data capture and retrieval.

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
- [Changelog – Documentation Updates](./CHANGELOG.md)

---

## Audience and Context

- **API Documentation** → Intended for developers integrating and maintaining backend services  
- **User Guide** → Designed for field consultants with limited technical background  
- **Editing Sample** → Demonstrates clarity improvement and ambiguity resolution  
- **Style Guide** → Demonstrates approach to maintaining consistency in documentation
- **Changelog** → Intended for internal stakeholders to track documentation updates and maintenance over time    

---

## Editorial Approach

The documentation samples focus on:

- Improving clarity without altering technical intent  
- Structuring information for usability and readability  
- Resolving ambiguous or unclear technical statements  
- Maintaining consistency across documents  

---

## Documentation Maintenance

- [Changelog](change-log.md)

---

## Tools and Workflow

- **Version Control:** Git/GitHub for managing changes and collaboration  
- **Markup:** Markdown (CommonMark) for structured and portable documentation  
- **Standards:** Based on the Microsoft Writing Style Guide and internal consistency guidelines  
- **API Validation:** Documentation structured using realistic request and response patterns, informed by typical API workflows  

---

## Note

All samples are based on prior project experience and are anonymized for demonstration purposes.
