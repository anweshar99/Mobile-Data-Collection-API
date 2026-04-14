# Mobile Data Collection API

## Overview
This API supports a mobile application used by field consultants to record and manage farmer data across Farmer Producer Organizations (FPOs). It is designed for efficient data capture and reduces dependency on manual documentation.

---

## Audience
Developers and technical team members responsible for integrating and maintaining the application.

---

## Base URL
https://api.farmerdata.app/v1

---

## Authentication
## Endpoints

### 1. Submit Farmer Data

**POST** `/collect-data`

**Description:**  
Creates a new farmer record in the system.

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

| Parameter  | Type   | Description        |
| ---------- | ------ | ------------------ |
| location   | string | Filter by location |
| start_date | date   | Filter from date   |

{
  "status": "success",
  "data": [
    {
      "farmer_id": "FPO12345",
      "name": "Ramesh Das",
      "crop_type": "Rice"
    }
  ]
}

{
  "status": "error",
  "message": "Invalid farmer ID"
}

| Code | Meaning      |
| ---- | ------------ |
| 400  | Bad request  |
| 401  | Unauthorized |
| 500  | Server error |

