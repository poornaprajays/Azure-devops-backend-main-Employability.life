# 🚀 Employability Life Azure DevOps Backend

[![Node.js](https://img.shields.io/badge/Node.js-18+-green.svg)](https://nodejs.org/)
[![NestJS](https://img.shields.io/badge/NestJS-10.0.0-red.svg)](https://nestjs.com/)
[![TypeORM](https://img.shields.io/badge/TypeORM-10.0.2-blue.svg)](https://typeorm.io/)
[![MySQL](https://img.shields.io/badge/MySQL-8.0+-orange.svg)](https://www.mysql.com/)
[![License](https://img.shields.io/badge/License-UNLICENSED-lightgrey.svg)](LICENSE)
[![GitHub issues](https://img.shields.io/github/issues/poornaprajays/Azure-devops-backend-main-Employability.life)](https://github.com/poornaprajays/Azure-devops-backend-main-Employability.life/issues)
[![GitHub pull requests](https://img.shields.io/github/issues-pr/poornaprajays/Azure-devops-backend-main-Employability.life)](https://github.com/poornaprajays/Azure-devops-backend-main-Employability.life/pulls)
[![GitHub stars](https://img.shields.io/github/stars/poornaprajays/Azure-devops-backend-main-Employability.life?style=social)](https://github.com/poornaprajays/Azure-devops-backend-main-Employability.life)

A robust NestJS backend application for the Employability Life Azure DevOps project, featuring user authentication, user management, and API endpoints built with TypeScript and MySQL.

## ✨ Features

- 🔐 **Authentication Module**: Secure login and user authentication using bcrypt
- 👤 **User Management**: CRUD operations for user entities with TypeORM
- 👋 **Hello World Endpoint**: Simple API endpoint for testing
- 🗄️ **MySQL Database Integration**: Persistent data storage with TypeORM
- 🧪 **Comprehensive Testing**: Unit and E2E tests with Jest
- 📦 **Modular Architecture**: Clean, scalable NestJS module structure

## 📋 Table of Contents

- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Configuration](#configuration)
- [Running the Application](#running-the-application)
- [API Endpoints](#api-endpoints)
- [Try the API](#try-the-api)
- [Testing](#testing)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)

## 🛠️ Prerequisites

Before running this application, make sure you have the following installed:

- **Node.js** (version 18 or higher) - [Download here](https://nodejs.org/)
- **npm** (comes with Node.js)
- **MySQL** (version 8.0 or higher) - [Download here](https://www.mysql.com/)

## 📦 Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/poornaprajays/Azure-devops-backend-main-Employability.life.git
   cd employability-life-azure-devops-backend-main
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

## ⚙️ Configuration

1. **Set up the database:**
   - Create a MySQL database/schema for the application
   - Update the database connection details in `src/app.module.ts`

2. **Environment variables:**
   - Create a `.env` file in the root directory (if not present)
   - Configure your database credentials and other environment-specific settings

## 🚀 Running the Application

### Development Mode
```bash
<<<<<<< HEAD
git clone https://github.com/poornaprajays/Azure-devops-backend-main-Employability.life.git
cd azure-devops-backend
=======
npm run start:dev
```
The server will start with hot-reload enabled on `http://localhost:4000`

### Production Mode
```bash
npm run build
npm run start:prod
>>>>>>> 2e3b18d (Enhance README with interactive features, badges, and API examples)
```

### Debug Mode
```bash
npm run start:debug
```

## 📡 API Endpoints

### Authentication
- `POST /auth/login` - User login

### Hello
- `GET /hello` - Returns a hello world message

### User Management
- User-related endpoints (check `src/user/` for details)

For detailed API documentation, refer to the Swagger/OpenAPI specs or the controller files.

## 🎮 Try the API

Once the server is running, you can test the endpoints using curl or any HTTP client:

### Test the Hello Endpoint
```bash
curl http://localhost:4000/hello
```
**Expected Response:**
```json
"Hello World"
```

### Login (Example)
```bash
curl -X POST http://localhost:4000/auth/login \
  -H "Content-Type: application/json" \
  -d '{"username": "your_username", "password": "your_password"}'
```

> 💡 **Tip**: Replace `your_username` and `your_password` with actual credentials. Check the login DTO in `src/auth/login.dto.ts` for the exact structure.

### Interactive Testing
- Use [Postman](https://www.postman.com/) or [Insomnia](https://insomnia.rest/) for a GUI experience
- Or try the built-in Swagger UI if configured (usually at `http://localhost:4000/api`)

<<<<<<< HEAD
You should see a 'Hey Azure here' message indicating that the server is running successfully.
=======
## 🧪 Testing

### Unit Tests
```bash
npm run test
```

### E2E Tests
```bash
npm run test:e2e
```

### Test Coverage
```bash
npm run test:cov
```

## 📁 Project Structure

```
src/
├── app.controller.ts          # Main app controller
├── app.module.ts              # Root application module
├── app.service.ts             # Main app service
├── main.ts                    # Application entry point
├── auth/                      # Authentication module
│   ├── auth.controller.ts
│   ├── auth.module.ts
│   ├── auth.service.ts
│   └── login.dto.ts
├── hello/                     # Hello world module
│   ├── hello.controller.ts
│   └── hello.controller.spec.ts
└── user/                      # User management module
    ├── user.entity.ts
    ├── user.module.ts
    └── user.service.ts
test/
├── app.e2e-spec.ts
└── jest-e2e.json
```

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the UNLICENSED License - see the [LICENSE](LICENSE) file for details.

---

Made with ❤️ using [NestJS](https://nestjs.com/)

### E2E Tests
```bash
npm run test:e2e
```

### Test Coverage
```bash
npm run test:cov
```

## 📁 Project Structure

```
src/
├── app.controller.ts          # Main app controller
├── app.module.ts              # Root application module
├── app.service.ts             # Main app service
├── main.ts                    # Application entry point
├── auth/                      # Authentication module
│   ├── auth.controller.ts
│   ├── auth.module.ts
│   ├── auth.service.ts
│   └── login.dto.ts
├── hello/                     # Hello world module
│   ├── hello.controller.ts
│   └── hello.controller.spec.ts
└── user/                      # User management module
    ├── user.entity.ts
    ├── user.module.ts
    └── user.service.ts
test/
├── app.e2e-spec.ts
└── jest-e2e.json
```

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the UNLICENSED License - see the [LICENSE](LICENSE) file for details.

---

Made with ❤️ using [NestJS](https://nestjs.com/)
>>>>>>> 2e3b18d (Enhance README with interactive features, badges, and API examples)
