# Selenium-Test-Automation-Framework

## Overview
This is a comprehensive Selenium Automation Framework built with a variety of powerful features aimed at enhancing the testing experience. The framework is designed to support parallel test execution, extensive reporting, and easy integration with multiple tools and services.

### Key Features:
- **Parallel Test Execution**: Tests can be run in parallel across multiple threads or machines for faster execution.
- **Reading Configurations from Properties Files**: External configurations are read from properties files to make the framework more flexible and customizable.
- **Extent and Allure Reporting**: Integration with Extent and Allure reports for detailed and visually appealing test reports.
- **Sending Test Reports via Email**: Automatically sends test reports via email, including HTML attachments.
- **Logging Mechanisms**: Comprehensive logging support to capture detailed logs of test execution for debugging and analysis.
- **Video Recording and Screenshots for Test Cases**: Video recording and automatic screenshot capturing for each test case for better traceability.
- **Reading Test Data from Various Sources**: Ability to read test data from different formats such as Excel, CSV, JSON, and others.
- **Base Utility Functions**: Core utility functions for enhanced maintainability, including handling waits, element interactions, etc.
- **WebUI Keyword-Based Approach**: A keyword-driven approach for common WebUI functions such as clicking, typing, and navigating.
- **Teams Notifications for Test Reports**: Automatically send test results to Microsoft Teams channels for easy team collaboration.
- **Running Tests on Selenium Grid (Remote Execution)**: Ability to run tests on Selenium Grid, enabling remote execution across multiple environments.
- **Retry Mechanism for Failed Tests**: Integration with TestNG’s retry mechanism to automatically re-run failed tests for increased reliability.

## Setup and Installation

### Prerequisites
1. Java (JDK 21)
2. Maven
3. TestNG
4. Selenium WebDriver
5. Extent Reports, Allure, and other dependencies configured in `pom.xml`
6. Microsoft Teams API (for notifications)
7. Selenium Grid (for remote execution)

### Steps to Set Up
1. Clone the repository:
    ```bash
    git clone <repository-url>
    ```
2. Navigate to the project folder:
    ```bash
    cd <project-directory>
    ```
3. Install dependencies using Maven:
    ```bash
    mvn clean install
    ```
4. Update configuration files as needed:
    - `config.properties` for general settings.
    - `testData.xlsx`, `testData.csv`, or `testData.json` for test data sources.

### Running Tests
To run tests:
```bash
mvn test -DsuiteXmlFile=testng.xml
