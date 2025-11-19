AI-Enhanced Test Automation Dashboard

A lightweight but powerful test automation platform that combines Selenium UI testing, a .NET 8 Web API, PostgreSQL, and AI-powered analysis. The system executes automated browser tests, stores results in a database, and uses AI to analyze failures or generate new test cases.

🎯 Project Purpose

This project aims to create an intelligent, modern test automation backend that:

Runs Selenium WebDriver tests through an API

Stores test cases and execution results (including errors) in PostgreSQL

Uses AI for root-cause analysis when a test fails

Generates new Selenium test cases from natural-language instructions

Provides a clean backend architecture that can later be extended with a UI dashboard

This project demonstrates how traditional UI testing can be enhanced with AI and data-driven insights.

🧱 Architecture Overview
/src
  /API                → ASP.NET Web API
  /Core               → Models & Interfaces
  /Infrastructure     → EF Core, DbContext, Migrations
  /Services           → Test Execution + AI Integration
  /SeleniumTests      → WebDriver scripts
/docker
  docker-compose.yml  → PostgreSQL setup

  
🗃️ Database Entities

TestCase — Stores test definitions
TestRun — Stores execution results
AIAnalysis — AI-generated insights for failed tests

🤖 AI Features
✔ AI Error Analysis

Explains failures, identifies potential root causes, and suggests improved locators or fixes.

✔ AI Test Case Generation

Converts natural-language requests into structured Selenium test cases and C# automation code.

🛠️ Technology Stack

C# / .NET 8

ASP.NET Web API

PostgreSQL + EF Core

Selenium WebDriver

OpenAI API

Docker

🚀 Getting Started
1. Start PostgreSQL (Docker)
docker compose up -d
2. Run the API
cd src/API
dotnet run

Swagger available at:

https://localhost:5001/swagger
📌 Roadmap

Test execution service (Selenium)

AI analysis endpoint

AI test case generator

Optional Blazor dashboard

📄 License

MIT

