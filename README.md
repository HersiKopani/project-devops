# project-devops

A simple full-stack example: a Spring Boot API and an Angular frontend that calls it.

## Structure

- `backend/` — Spring Boot app exposing `GET /api/hello`, which returns `hello world`.
- `frontend/` — Angular app that calls `/api/hello` and displays the result.

## Running locally

### Backend

```bash
cd backend
./mvnw spring-boot:run
```

Runs on http://localhost:8080. Verify with:

```bash
curl http://localhost:8080/api/hello
```

### Frontend

```bash
cd frontend
npm install
npx ng serve
```

Runs on http://localhost:4200 and calls the backend at `http://localhost:8080/api/hello`.
