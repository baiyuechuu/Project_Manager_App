# Project_Manager_App

A Flutter application for managing projects, tasks, and teams with a clean, scalable architecture.

## Features

### Authentication
- [ ] Welcome Page
- [ ] Login Page
- [ ] Register Page

### Project Management
- [ ] Project List Page
- [ ] Project Detail Page

### Task Management
- [ ] Project Task List Page
- [ ] Project Task Detail Page
- [ ] Project Task Add Page
- [ ] Project Task Edit Page

### Team Management
- [ ] Add Member Page
- [ ] Add Team Page

## Project Structure

The `lib` folder is organized following clean architecture principles for better maintainability and scalability:

```
lib/
├── main.dart                    # App entry point
├── core/                        # Core functionality
│   ├── constants/              # App-wide constants (colors, strings, API endpoints)
│   ├── utils/                  # Helper functions and utilities
│   ├── services/               # API services, local storage, etc.
│   └── themes/                 # App themes and styling
├── data/                       # Data layer
│   ├── models/                 # Data models and entities
│   ├── repositories/           # Data access layer
│   └── datasources/            # Remote and local data sources
├── presentation/               # Presentation layer
│   ├── pages/                  # App screens/pages
│   │   ├── auth/              # Authentication pages (Welcome, Login, Register)
│   │   ├── projects/          # Project-related pages (List, Detail)
│   │   ├── tasks/             # Task-related pages (List, Detail, Add, Edit)
│   │   └── teams/             # Team-related pages (Add Member, Add Team)
│   ├── widgets/               # Reusable UI components
│   │   ├── common/            # Common widgets used across the app
│   │   ├── forms/             # Custom form components
│   │   └── cards/             # Project cards, task cards, etc.
│   └── providers/             # State management (Provider, Riverpod, etc.)
└── routes/                     # App navigation and routing
```

## Development Guidelines

### Folder Organization
- **core/**: Contains app-wide utilities, constants, and services
- **data/**: Handles data management, API calls, and local storage
- **presentation/**: Contains UI components, pages, and state management
- **routes/**: Manages app navigation and routing logic

### File Naming Convention
- Use snake_case for file names
- Use descriptive names that clearly indicate the file's purpose
- Group related files in appropriate folders

### Architecture Benefits
- **Separation of Concerns**: Each layer has a specific responsibility
- **Scalability**: Easy to add new features and pages
- **Maintainability**: Clear structure makes code easier to understand and modify
- **Testability**: Well-organized code is easier to unit test
- **Reusability**: Common widgets and utilities can be shared across the app
