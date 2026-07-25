# CRUD Cycle & Roster Registration Log

## Task 1: CRUD Cycle

### Step 1: POST /api/posts (Create)
```http
HTTP/1.1 201 Created
Date: Sat, 25 Jul 2026 19:04:14 GMT
Content-Type: application/json; charset=utf-8

{
  "id": 33,
  "title": "exploring",
  "body": "full cycle",
  "author": "tareq",
  "created_at": "2026-07-25 19:04:14"
}HTTP/1.1 200 OK
Date: Sat, 25 Jul 2026 19:05:12 GMT
Content-Type: application/json; charset=utf-8

{
  "id": 33,
  "title": "exploring",
  "body": "full cycle",
  "author": "tareq",
  "created_at": "2026-07-25 19:04:14"
}HTTP/1.1 200 OK
Date: Sat, 25 Jul 2026 19:05:20 GMT
Content-Type: application/json; charset=utf-8

{
  "id": 33,
  "title": "exploring - edited",
  "body": "full cycle",
  "author": "tareq",
  "created_at": "2026-07-25 19:04:14"
}HTTP/1.1 200 OK
Date: Sat, 25 Jul 2026 19:05:24 GMT
Content-Type: application/json; charset=utf-8

{
  "deleted": true,
  "id": 33,
  "proof": "GET /api/posts/33 will now return 404 — that is real persistence"
}HTTP/1.1 404 Not Found
Date: Sat, 25 Jul 2026 19:05:28 GMT
Content-Type: application/json; charset=utf-8

{
  "error": "post 33 not found"
}HTTP/1.1 201 Created
Date: Sat, 25 Jul 2026 19:08:17 GMT
Content-Type: application/json; charset=utf-8

{
  "username": "tareq",
  "name": null,
  "created_at": "2026-07-25 19:08:17",
  "next_step": "POST /api/students/tareq/contacts to add your first contact"
}HTTP/1.1 409 Conflict
Date: Sat, 25 Jul 2026 19:08:23 GMT
Content-Type: application/json; charset=utf-8

{
  "error": "username 'tareq' is already registered — 409 means: conflict with existing state"
}
