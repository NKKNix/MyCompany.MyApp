# 🧱 MyCompany.MyApp – .NET 9 Clean Architecture Template

This repository is a **.NET 9 Clean Architecture Template** designed for enterprise-level applications.  
It serves as a scalable starting point for building robust APIs or backend systems using modern .NET practices.

---

## 🎯 Purpose

This template provides a pre-structured solution for:

- Multi-project .NET applications
- Scalable web APIs
- Separation of concerns (Clean Architecture)
- Testable business logic
- Easy integration with CI/CD

## 🗂️ Project Structure

```text
MyCompany.MyApp/
├── src/
│   ├── MyCompany.MyApp.Web/          # Web API entry point
│   │   ├── Controllers/              # ASP.NET Controllers
│   │   ├── Program.cs                # Main app startup
│   │   └── MyCompany.MyApp.Web.csproj
│   │
│   ├── MyCompany.MyApp.Core/         # Domain layer
│   │   ├── Entities/                 # Domain models
│   │   ├── Interfaces/               # Service/Repo interfaces
│   │   └── MyCompany.MyApp.Core.csproj
│   │
│   ├── MyCompany.MyApp.Services/     # Business logic layer
│   │   ├── Implementations/          # Service implementations
│   │   └── MyCompany.MyApp.Services.csproj
│   │
│   ├── MyCompany.MyApp.Data/         # Data access layer
│   │   ├── DbContext/                # EF Core context
│   │   ├── Repositories/             # Repository pattern
│   │   └── MyCompany.MyApp.Data.csproj
│   │
│   └── MyCompany.MyApp.Shared/       # Shared utilities
│       ├── Extensions/               # Extension methods
│       ├── Constants/                # Global constants
│       └── MyCompany.MyApp.Shared.csproj
│
├── tests/
│   └── MyCompany.MyApp.Tests/        # xUnit test project
│       ├── TestHelpers/              # Mocks, fixtures
│       └── MyCompany.MyApp.Tests.csproj
│
├── MyCompany.MyApp.sln               # Solution file
├── README.md                         # Project documentation
└── .gitignore                        # Git ignore rules


## 🔧 Technologies Used

- [.NET 9 SDK](https://dotnet.microsoft.com/)
- ASP.NET Core Web API
- Entity Framework Core (optional)
- xUnit for Unit Testing
- Clean Architecture Principles
- Git for version control

---

## 🚀 How to Use This Template

1. Clone the repo:
   ```bash
   git clone https://github.com/your-org/your-repo-name.git
2. Run the application
   ```bash
   dotnet run --project src/MyCompany.MyApp.Web
3. Start building features by adding to:
   ```bash
   Services for business logic
   Core for contracts & models
   Data for persistence
   Web for API endpoints
  
4. Running Tests
   ```bash
   dotnet test
