# REST API README Sample

## Introduction
This API allows developers to access and manipulate user data and project settings programmatically.

## Base URL
`https://api.example.com/v1`

## Authentication
All API requests require an API Key to be included in the header.
`Authorization: Bearer YOUR_API_KEY`

## Endpoints

### 1. Get User Profile
Retrieves the public profile of a user.

- **URL:** `/users/:id`
- **Method:** `GET`
- **Success Response:**
  - **Code:** 200 OK
  - **Content:** `{ "id": 12, "name": "Erwin", "role": "admin" }`

### 2. Create Project
Creates a new project under the user's account.

- **URL:** `/projects`
- **Method:** `POST`
- **Data Params:** `{ "title": "New App", "private": true }`
- **Success Response:**
  - **Code:** 201 Created

## Error Codes
- **401:** Unauthorized (Invalid API Key)
- **404:** Resource Not Found
- **500:** Server Error
