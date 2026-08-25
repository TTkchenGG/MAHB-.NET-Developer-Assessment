# MAHB-.NET-Developer-Assessment

# Payroll Management System

## Overview

Payroll Management System developed using ASP.NET Core Web API, Dapper, SQL Server, React, Axios and Bootstrap.

The application allows users to manage employee information and calculate payroll based on working days and birthday bonus rules.

---

## Features

### Employee Management

- Create Employee
- View Employee List
- Search Employees
- Update Employee
- Delete Employee
- Archive Employee
- Unarchive Employee

### Employee Information

- Employee Number Generation
- Working Days Management
- Skillsets Management

### Payroll Calculation

- Calculate payroll within a date range
- Birthday bonus calculation
- Total pay calculation

---

## Technology Stack

### Backend

- ASP.NET Core Web API
- Dapper
- SQL Server
- FluentValidation
- Swagger
- xUnit

### Frontend

- React
- React Router
- Axios
- Bootstrap
- Vite

---
## Database Setup

1. Create a SQL Server database.
2. Run the provided SQL script in 'Database/Init.sql' to create the required tables.
3. Update the connection string in:

```text
CDN.Payroll.API/appsettings.json
```

Example:

```json
{
  "ConnectionStrings": {
    "DefaultConnection": "Your SQL Server Connection String"
  }
}
```
---

## Running the Backend

```bash
dotnet restore
dotnet build
dotnet run --project CDN.Payroll.API
```

Open Swagger:

```text
https://localhost:<port>/swagger
```

---

## Running the Frontend

```bash
cd payroll-ui
npm install
npm run dev
```

Open:

```text
http://localhost:5173
```

---

## Payroll Formula

```text
Working Day Pay
= Working Day Count × Daily Rate × 2

Birthday Bonus
= 1 Additional Day Pay

Total Pay
= Working Day Pay + Birthday Bonus
```


