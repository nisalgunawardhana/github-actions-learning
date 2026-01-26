# Sample Node.js Application

This is a simple Express.js application for learning GitHub Actions. Built with best practices for CI/CD workflows using GitHub Actions.

## Getting Started

### Install Dependencies

```bash
npm install
```

### Development

```bash
npm run dev
```

The app will start on `http://localhost:3000`

### Run Tests

```bash
npm test
```

### Linting

```bash
npm run lint
npm run lint:fix
```

## API Endpoints

### GET /
Returns welcome message

```bash
curl http://localhost:3000/
```

Response:
```json
{
  "message": "Welcome to GitHub Actions Learning App!",
  "status": "OK",
  "version": "1.0.0"
}
```

### GET /api/hello
Returns hello message

```bash
curl http://localhost:3000/api/hello?name=Alice
```

Response:
```json
{
  "message": "Hello, Alice!",
  "timestamp": "2024-01-03T12:00:00.000Z"
}
```

### GET /api/status
Returns application status

```bash
curl http://localhost:3000/api/status
```

Response:
```json
{
  "status": "healthy",
  "uptime": 123.45,
  "environment": "development"
}
```

### POST /api/data
Process text data

```bash
curl -X POST http://localhost:3000/api/data \
  -H "Content-Type: application/json" \
  -d '{"text":"hello"}'
```

Response:
```json
{
  "received": "hello",
  "length": 5,
  "uppercase": "HELLO"
}
```

### GET /health
Health check endpoint

```bash
curl http://localhost:3000/health
```

## Environment Variables

- `PORT` - Server port (default: 3000)
- `NODE_ENV` - Environment (development/production)

## Project Structure

```
sample-app/
├── src/
│   └── server.js          # Main application file
├── tests/
│   └── server.test.js     # Test suite
├── package.json           # Dependencies
└── README.md             # This file
```

## Testing

The application includes comprehensive tests using Jest and Supertest.

Run tests:
```bash
npm test
```

Run tests in watch mode:
```bash
npm run test:watch
```

## Building

```bash
npm run build
```

## Deployment

This app is designed to be deployed to Azure App Service:

1. Build: `npm run build`
2. Install: `npm install`
3. Start: `npm start`

The app includes a health check endpoint at `/health` which returns HTTP 200 when ready.

---

**Happy learning! 🎓**
