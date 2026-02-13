# API Specification

## Authentication
Admin access for managing portfolio content.
- `POST /api/auth/login` - Admin login (OAuth or Magic Link)
- `POST /api/auth/logout` - Admin logout
- `GET /api/auth/session` - Get current admin session

## Core Endpoints

### Projects
- `GET /api/projects` - List all projects (Public)
- `GET /api/projects/:slug` - Get project details by slug (Public)
- `POST /api/projects` - Create a new project (Admin Only)
- `PATCH /api/projects/:id` - Update project details (Admin Only)
- `DELETE /api/projects/:id` - Delete a project (Admin Only)

### Contact
- `POST /api/contact` - Submit a contact form message (Public)
- `GET /api/contact` - List contact messages (Admin Only)
- `DELETE /api/contact/:id` - Delete a contact message (Admin Only)

### Tech Stack / Metadata
- `GET /api/metadata` - Get global site metadata (Public)

## Request/Response Format

### Standard Success Response
```json
{
  "success": true,
  "data": { ... },
  "message": "Optional message"
}
```

### Error Response
```json
{
  "success": false,
  "error": {
    "code": "ERROR_CODE",
    "message": "Human readable message"
  }
}
```

## Status Codes
- 200: Success
- 201: Created
- 400: Bad Request
- 401: Unauthorized (Admin only)
- 403: Forbidden
- 404: Not Found
- 500: Server Error
