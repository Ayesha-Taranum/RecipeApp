# Modern Recipe Management System

A full-stack application for managing and organizing recipes with a modern tech stack.

## Tech Stack

### Backend
- Java 8
- Spring Boot 2.1.3
- Spring Data JPA
- H2 In-Memory Database
- Maven

### Frontend
- Angular
- TypeScript
- Node.js

## Features

- **Recipe Management**: Create, read, update, and delete recipes
- **Ingredient Tracking**: Manage ingredients for each recipe
- **Real-time Updates**: Instant reflection of changes across the application
- **Responsive Design**: Works seamlessly on desktop and mobile devices
- **In-Memory Database**: Fast and efficient data storage with H2

## Project Structure

```
recipe-app/
├── server/                 # Spring Boot backend
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/      # Java source code
│   │   │   └── resources/ # Configuration files
│   │   └── test/          # Test files
│   └── pom.xml            # Maven configuration
└── client/                # Angular frontend
    ├── src/
    │   ├── app/          # Angular components
    │   └── assets/       # Static resources
    └── package.json      # Node.js dependencies
```

## Getting Started

### Prerequisites
- Java 8 or higher
- Node.js 12 or higher
- Maven 3.6 or higher

### Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd recipe-app
```

2. Start the backend server:
```bash
cd server
./mvnw spring-boot:run
```

3. Start the frontend application:
```bash
cd client
npm install
npm start
```

4. Access the application:
- Backend API: http://localhost:8080
- Frontend: http://localhost:4200
- H2 Console: http://localhost:8080/h2-console

## API Endpoints

- `GET /api/recipes` - List all recipes
- `POST /api/recipes` - Create a new recipe
- `GET /api/recipes/{id}` - Get a specific recipe
- `PUT /api/recipes/{id}` - Update a recipe
- `DELETE /api/recipes/{id}` - Delete a recipe

## Development

### Backend Development
- Run tests: `./mvnw test`
- Build JAR: `./mvnw clean package`
- Code formatting: `./mvnw spotless:apply`

### Frontend Development
- Run tests: `npm test`
- Build production: `npm run build`
- Lint code: `npm run lint`

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
