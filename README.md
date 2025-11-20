📘 Contract Monthly Claim System

A modern ASP.NET Core MVC application designed to streamline, automate, and digitize the contract lecturer monthly claim process. The system simplifies claim submissions, supports administrative validation, and offers centralized reporting tools for improved transparency and efficiency.

📑 Table of Contents

Overview

Features

System Architecture

Technology Stack

Installation & Setup

Database Configuration

How It Works

Project Structure

Screenshots (Optional)

Future Enhancements

Author

📝 Overview

The Contract Monthly Claim System was developed to automate and manage the monthly claim process for contract lecturers.
This system replaces manual processes such as spreadsheets, emails, and paper forms with a fully digital workflow that ensures accuracy, security, and convenience.

The system supports:

Lecturer claim submissions

Admin review & approval

Automatic calculations

Digital record keeping

Reporting and dashboard insights

⭐ Features
👨‍🏫 Lecturer Features

Submit monthly claims online

Upload or input hours worked per module

Track claim approval status

Review historical claims

🛠️ Admin Features

View pending, approved, and rejected claims

Validate submitted claim details

Approve or reject lecturer submissions

Generate reports

Manage lecturer information and user accounts

📊 System Features

Automated total calculations

SQL database integration

Role-based access (Admin / Lecturer)

Clean, modern user interface

Dashboard insights (workload, claims, totals)

🏗️ System Architecture

The system is built using a layered architecture:

Presentation Layer (Views)
│
├── MVC Controllers
│
├── Business Logic Layer
│
└── Data Access Layer (Repository Pattern + EF Core)
      └── SQL Server Database


This structure improves maintainability, scalability, and separation of concerns.

🧰 Technology Stack
Category	Technology
Framework	ASP.NET Core MVC
Language	C#
Database	SQL Server
ORM	Entity Framework Core
Authentication	ASP.NET Core Identity
Frontend	Bootstrap 5, HTML, CSS
IDE	Visual Studio 2022
Version Control	Git & GitHub

⚙️ Installation & Setup
1️⃣ Clone the Repository
git clone https://github.com/YourUsername/ContractMonthlyClaimSystem.git

2️⃣ Open the Project

Open the solution file (.sln) in Visual Studio 2022.

3️⃣ Restore Dependencies

Visual Studio will automatically restore NuGet packages.
If not, run:

dotnet restore

🗄️ Database Configuration
Update the Connection String

In appsettings.json, update your connection string:

"ConnectionStrings": {
  "DefaultConnection": "Server=YOUR_SERVER;Database=ClaimsDB;Trusted_Connection=True;MultipleActiveResultSets=true;TrustServerCertificate=true;"
}
Apply Migrations
dotnet ef database update

🔄 How It Works (Workflow)

Lecturer logs into the system

Lecturer submits a new claim for the month

System validates the submission

Admin reviews the claim

Admin approves or rejects

System stores and updates records

Reports and dashboards are updated automatically