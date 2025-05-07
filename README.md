# SterlingB E-Commerce Application

This is a modern e-commerce application built using .NET Core with a clean architecture approach. The solution follows best practices and is structured in multiple layers for better maintainability and scalability.

## Project Structure

The solution is organized into the following projects:

- **ECommerce.Web**: The presentation layer containing the web API and UI components
- **ECommerce.Application**: Contains business logic and application services
- **ECommerce.Domain**: Contains domain entities, interfaces, and business rules
- **ECommerce.Infrastructure**: Implements data access, external services, and infrastructure concerns

## Prerequisites

## Getting Started

1. Clone the repository:
   ```bash
   git clone https://github.com/Bholajie/STERLINGPRO.git
   cd SterlingB
   ```

2. Open the solution:
   - Using Visual Studio: Open `Ecommerce.sln`
   - Using VS Code: Open the folder and select the solution file

3. Restore NuGet packages:
   ```bash
   dotnet restore
   ```

4. Update the connection string in `appsettings.json` to point to your SQL Server instance.

5. Run the database migrations:
   ```bash
   cd ECommerce.Web
   dotnet ef database update
   ```

6. Run the application:
   ```bash
   dotnet run
   ```

The application will be accessible at:
- Main application: [https://localhost:7023/index.html](https://localhost:7023)
- Login page: [https://localhost:7023/login.html](https://localhost:7023/login.html)

## API Documentation

Once the application is running, you can access the Swagger documentation at:
- `https://localhost:7023/swagger`

## Development

### Building the Solution
```bash
dotnet build
```

### Running Tests
```bash
dotnet test
```

## Project Architecture

This project follows Clean Architecture principles:

- **Domain Layer**: Contains enterprise business rules and entities
- **Application Layer**: Contains business rules and orchestrates the flow of data
- **Infrastructure Layer**: Implements interfaces defined in the application layer
- **Web Layer**: Contains the API controllers and UI components 