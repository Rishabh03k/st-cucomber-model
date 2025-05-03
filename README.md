# 🧪 Cucumber + Asana Automation Testing Framework

A modern BDD automation framework using **Cucumber**, **Selenium**, and **Java**, integrated with **Asana API** to automatically create tasks for failed scenarios and generate rich test reports using **Allure** or **ExtentReports**.

---

## ⚙️ Setup Instructions

### 🛠 Prerequisites

- Java 11 or higher
- Maven
- Chrome + ChromeDriver
- Git
- [Asana Personal Access Token](https://app.asana.com/0/developer-console)

### 📥 Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/asana-cucumber-automation.git
   cd asana-cucumber-automation
2.Add your Asana API token
In utils/AsanaIntegration.java, replace:
private static final String PERSONAL_ACCESS_TOKEN = "your-asana-token";

3.Install Maven dependencies:
mvn clean install

#Running Tests
Run All Tests
mvn test
#Run Tests by Tag
mvn test -Dcucumber.filter.tags="@login"


# PRoject Structure
asana-cucumber-automation/
│
├── src/
│   └── test/
│       └── java/
│           ├── features/                # Gherkin feature files (.feature)
│           ├── stepdefinitions/         # Step definitions for steps
│           ├── runners/                 # Cucumber test runners
│           ├── pages/                   # Page Object Model classes
│           └── utils/                   # Helpers like Asana integration, drivers
│
├── reports/                             # Allure or Extent test reports
├── pom.xml                              # Maven project config and dependencies
└── README.md                            # Project documentation

 #Test Report
1. Allure Report
2.2. Extent Report (Optional)
