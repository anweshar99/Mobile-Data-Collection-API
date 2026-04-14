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

All requests require a Bearer Token:
Authorization: Bearer <access_token>

---

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
####Response
{
  "status": "success",
  "message": "Farmer data recorded successfully",
  "record_id": "REC67890"
}
### 2. Fetch Farmer Records

**GET** `/farmer-records`

**Description:**  
Retrieves farmer records based on filters.

#### Query Parameters

| Parameter   | Type   | Description        |
|------------|--------|--------------------|
| location   | string | Filter by location |
| start_date | date   | Filter from date   |

#### Response
```json
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
### 3. Update Farmer Record

**PUT** `/update-record/{record_id}`

**Description:**  
Updates an existing farmer record.

#### Request Body
```json
{
  "crop_type": "Wheat",
  "land_size_acres": 3
}
{
  "status": "success",
  "message": "Record updated successfully"
}
