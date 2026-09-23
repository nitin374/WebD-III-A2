# Student Management REST API

A basic REST API made with Node.js and Express.js. Student data is stored in an array, so changes reset when the server restarts.

## Run the project

```bash
npm install
npm start
```

Server URL: `http://localhost:3000`

## Test in Postman

For POST and PUT, select **Body > raw > JSON** and add the header `Content-Type: application/json`.

| Method | URL | Purpose |
|---|---|---|
| GET | `http://localhost:3000/students` | View all students |
| GET | `http://localhost:3000/students/1` | View student with ID 1 |
| POST | `http://localhost:3000/students` | Add a student |
| PUT | `http://localhost:3000/students/1` | Update student with ID 1 |
| DELETE | `http://localhost:3000/students/1` | Delete student with ID 1 |

### POST body example

```json
{
  "name": "Nitin",
  "course": "BTech"
}
```

### PUT body example

```json
{
  "name": "Nitin Kumar",
  "course": "BCA"
}
```
