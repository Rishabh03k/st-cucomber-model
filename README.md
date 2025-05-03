# 🧪 Cucumber + Asana Automation Framework

[![Build Status](https://img.shields.io/badge/build-passing-brightgreen)](#)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](#)
[![Test Automation](https://img.shields.io/badge/tested-with%20love-green)](#)

> ⚡ A powerful BDD automation testing framework built using **Cucumber** and **Selenium**, integrated with the **Asana API** to auto-create tasks for failed test cases. Designed for agile teams to enhance test visibility and real-time issue tracking.

---

## 📌 Overview

This framework combines:
- 🧪 **Behavior-Driven Development (BDD)** via Cucumber
- 🖥️ **Web UI Automation** using Selenium WebDriver
- 🔄 **Asana Integration** for automated task creation on failure
- 📊 **Test Reporting** with Allure or ExtentReports
- 🚀 **CI/CD Ready** with support for GitHub Actions, Jenkins, etc.

Whether you're part of a QA team or a solo tester, this framework helps track bugs instantly and maintain robust, scalable test suites.

---

## 🧱 Project Structure

asana-cucumber-automation/
│
├── src/
│   └── test/
│       └── java/
│           ├── features/                # Gherkin feature files (.feature)
│           │   └── login.feature
│           │
│           ├── stepdefinitions/         # Step definitions for feature steps
│           │   └── LoginSteps.java
│           │
│           ├── runners/                 # Cucumber test runner classes
│           │   └── TestRunner.java
│           │
│           ├── pages/                   # Page Object Model classes
│           │   └── LoginPage.java
│           │
│           └── utils/                   # Asana integration, config helpers, etc.
│               ├── AsanaIntegration.java
│               └── DriverManager.java
│
├── reports/                             # Generated test reports (Allure/Extent)
│
├── pom.xml                              # Maven dependencies and build config
├── .gitignore                           # Git ignored files
└── README.md                            # Project overview and instructions
