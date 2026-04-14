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

### 1. Submit Farmer Data

**POST** `/collect-data`

**Description:**  
Creates a new farmer record.

#### Request Body
```json
{
  "farmer_id": "FPO12345",
  "name": "Ramesh Das",
  "crop_type": "Rice",
  "land_size_acres": 2.5,
  "location": "Nadia, West Bengal",
  "collection_date": "2023-09-15"
}

{
  "status": "success",
  "message": "Farmer data recorded successfully",
  "record_id": "REC67890"
}

