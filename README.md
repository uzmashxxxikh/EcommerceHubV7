# 🛒 EcommerceHubV7 – Hybrid Automation Framework

<p align="center">
  <strong>A scalable, data-driven web automation framework built with Java, Selenium WebDriver, and TestNG.</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white" />
  <img src="https://img.shields.io/badge/Selenium-43B02A?style=for-the-badge&logo=selenium&logoColor=white" />
  <img src="https://img.shields.io/badge/TestNG-FF6C37?style=for-the-badge&logo=testng&logoColor=white" />
  <img src="https://img.shields.io/badge/Maven-C71A36?style=for-the-badge&logo=apachemaven&logoColor=white" />
  <img src="https://img.shields.io/badge/ExtentReports-Reporting-blue?style=for-the-badge" />
</p>

---

## 📌 Overview

**EcommerceHubV7** is a Java-based Hybrid Test Automation Framework designed to automate end-to-end testing of an e-commerce web application.

The framework uses Selenium WebDriver for browser automation and TestNG for test organization, execution, grouping, and parallel testing. It incorporates data-driven testing capabilities, reusable automation components, and ExtentReports for generating detailed execution reports.

The goal of this project is to improve test efficiency, reduce repetitive manual testing, and establish a maintainable automation solution that supports multiple browsers and different testing scenarios.

## ✨ Key Features

| Feature | Description |
|---|---|
| 🌐 Cross-Browser Testing | Supports Chrome, Firefox, and Microsoft Edge. |
| 🧪 Regression Testing | Executes a dedicated regression test suite. |
| 📊 Data-Driven Testing | Supports external test data using Apache POI. |
| 📈 Automated Reporting | Generates detailed test execution reports using ExtentReports. |
| ⚡ Parallel Execution | Supports parallel test execution through TestNG. |
| 🔧 Reusable Components | Uses organized test cases and supporting utilities. |
| 📝 Logging | Integrates Log4j for application and execution logging. |
| 📧 Email Integration | Includes Apache Commons Email dependency for email-related functionality. |

## 🛠️ Technology Stack

| Technology | Purpose |
|---|---|
| Java | Primary programming language |
| Selenium WebDriver 4.51.0 | Web browser automation |
| TestNG 7.12.0 | Test execution and test management |
| Apache Maven | Dependency and project management |
| ExtentReports 5.1.2 | Test execution reporting |
| Apache POI 6.0.0 | Excel-based test data handling |
| Log4j 2.26.1 | Logging |
| Apache Commons Email 1.6.0 | Email functionality |

## 🧪 Automated Test Scenarios

The framework currently includes automation scenarios covering important e-commerce workflows:

- **Application Launch:** Validates that the application launches successfully.
- **User Authentication:** Tests user login functionality.
- **Data-Driven Login:** Executes login scenarios using external test data.
- **Shopping Cart:** Tests adding products to the shopping cart.
- **Wishlist:** Validates adding products to a wishlist.
- **Affiliate Management:** Tests affiliate-related functionality.
- **Purchase Workflow:** Automates the purchase completion process.

## 🌐 Cross-Browser Compatibility

The TestNG suite is configured to execute the automation scenarios across three major browsers.

| Browser | Support |
|---|---|
| Google Chrome | ✅ |
| Mozilla Firefox | ✅ |
| Microsoft Edge | ✅ |

The framework uses TestNG XML configuration to organize browser-specific test executions.

## 📂 Project Structure

The repository is organized around test automation, test data, reporting, and execution artifacts.

```text
EcommerceHubV7/
│
├── src/
│   └── test/
│       └── java/
│           ├── testCases/
│           ├── pageObjects/
│           ├── utilities/
│           └── ...
│
├── testData/                 # External test data
├── screenshots/              # Captured test screenshots
├── reports/                  # Test execution reports
├── logs/                     # Execution logs
├── test-output/              # TestNG output
├── target/                   # Maven build output
│
├── pom.xml                   # Maven dependencies
├── testng.xml                # TestNG suite configuration
├── .gitignore
└── README.md
```

*Note: The package-level folders above illustrate the intended organization. Adjust them to match the actual source folders in your repository.*

## ⚙️ Getting Started

Follow these instructions to set up the project locally.

### Prerequisites

Make sure the following tools are installed:

- Java Development Kit (JDK)
- Apache Maven
- Eclipse IDE or IntelliJ IDEA
- Google Chrome, Mozilla Firefox, or Microsoft Edge
- Git

### 1. Clone the Repository

```bash
git clone https://github.com/uzmashxxxikh/EcommerceHubV7.git
```

### 2. Navigate to the Project Directory

```bash
cd EcommerceHubV7
```

### 3. Import the Project

Import the project into Eclipse or IntelliJ IDEA as an existing Maven project.

Allow Maven to download and configure the required dependencies from `pom.xml`.

### 4. Configure Test Execution

Open `testng.xml` to review the test suite configuration.

The current configuration includes:

- Regression test group
- Chrome execution
- Firefox execution
- Edge execution
- TestNG listener for ExtentReports
- Parallel test execution configuration

### 5. Run the Automation Suite

Execute the following Maven command:

```bash
mvn clean test
```

Alternatively, right-click `testng.xml` in Eclipse and select **Run As → TestNG Suite**.

*Ensure your application URL and any required test credentials or test data are configured before execution.*

## 📊 Test Reporting

The framework integrates **ExtentReports** to provide a structured view of test execution results.

The reporting listener is configured through TestNG:

```xml
<listeners>
    <listener class-name="utilities.ExtentReportManager"/>
</listeners>
```

Reports can provide a convenient way to review:

- Test execution status
- Passed and failed test cases
- Execution details
- Failure information
- Test execution history, where configured

Generated reports and screenshots are maintained in the project's reporting and screenshot directories.

## 📸 Screenshots & Test Evidence

Screenshots and testing artifacts are maintained in the repository to provide visual evidence of the automation framework and its execution.

<!-- Add screenshots here once the actual image filenames are confirmed. -->

Examples of screenshots to showcase:

1. Test execution results
2. ExtentReports dashboard
3. Successful login scenario
4. Shopping cart workflow
5. Cross-browser execution

## 🚀 Future Enhancements

Potential improvements to expand the framework include:

- [ ] Integrate Jenkins or GitHub Actions for CI/CD execution.
- [ ] Expand API automation testing.
- [ ] Implement additional test coverage for checkout and payment workflows.
- [ ] Improve failure handling and automatic screenshot capture.
- [ ] Add more comprehensive test data management.
- [ ] Introduce automated test result notifications.
- [ ] Expand browser and environment configurations.

## 👩‍💻 Author

**Uzma Shaikh**

Computer Programming & Analysis | Software Development | Test Automation

- GitHub: [@uzmashxxxikh](https://github.com/uzmashxxxikh)
- Project Repository: [EcommerceHubV7](https://github.com/uzmashxxxikh/EcommerceHubV7)

---

<p align="center">
  <strong>Built with Java, Selenium WebDriver, and a passion for software quality. 🐈</strong>
</p>
