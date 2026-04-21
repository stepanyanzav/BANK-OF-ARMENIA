# Bank of Armenia Digital Banking Platform

## Prerequisites
1. **Docker** - Ensure that Docker is installed on your machine. You can download it from [Docker's official website](https://www.docker.com/get-started).
2. **Docker Compose** - Make sure Docker Compose is installed. It usually comes bundled with Docker for Windows and Mac. For Linux, you can install it as follows:
   ```bash
   sudo apt-get install docker-compose
   ```
3. **Node.js** - Install Node.js from [Node.js official website](https://nodejs.org/).
   - Verify installation:
   ```bash
   node -v
   npm -v
   ```

## Quick Start Guide
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/bank-of-armenia.git
   cd bank-of-armenia
   ```
2. Build and run the application:
   ```bash
   docker-compose up --build
   ```
3. Access the application in your web browser at `http://localhost:3000`

## Docker-Compose Commands
- **Starting the application:**
  ```bash
  docker-compose up
  ```
- **Stopping the application:**
  ```bash
  docker-compose down
  ```
- **Rebuilding the application:**
  ```bash
  docker-compose up --build
  ```
- **Viewing logs:**
  ```bash
  docker-compose logs -f
  ```

## Deployment Options
- **Local Deployment:** Work locally using Docker to develop and test features without impacting the production environment.
- **Cloud Deployment:** Use services like AWS, Azure, or Google Cloud for deploying the application in a production environment. Ensure to configure environment variables as needed.

## API Documentation
### Endpoints
- **GET /api/v1/accounts** - Retrieve the list of accounts.
- **POST /api/v1/accounts** - Create a new bank account.
- **GET /api/v1/accounts/:id** - Retrieve a specific bank account by ID.
- **PUT /api/v1/accounts/:id** - Update a specific bank account.
- **DELETE /api/v1/accounts/:id** - Delete a specific bank account.

### Authentication
Ensure to use `Bearer Token` in the Authorization header for accessing protected routes.

### Example Request
```bash
curl -X GET http://localhost:3000/api/v1/accounts -H 'Authorization: Bearer YOUR_TOKEN'
```

## Contact
For any questions or feedback, reach out to the development team via email at support@bankofarmenia.am.

---
*Last updated: 2026-04-21*