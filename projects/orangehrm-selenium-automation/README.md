# OrangeHRM Selenium Test Automation

## Project Overview

A Selenium WebDriver automation framework developed to validate the OrangeHRM web application's login functionality.

The project automates both successful and unsuccessful login scenarios using Java, Selenium WebDriver, TestNG, and Maven.

## Technologies Used

- Java 17
- Selenium WebDriver 4.48.0
- TestNG 7.11.0
- Maven
- ExtentReports 5.1.2
- Chrome Browser
- Page Object Model (POM)

## Automation Coverage

### 1. Successful Login
- Opens the OrangeHRM login page
- Enters valid username and password
- Clicks the Login button
- Verifies that the Dashboard is displayed

### 2. Invalid Login
- Enters valid username with an invalid password
- Clicks the Login button
- Verifies that the invalid credentials message is displayed
- Captures and validates the error message

## Framework Features

- Page Object Model (POM)
- Explicit Waits using WebDriverWait
- TestNG test execution
- Maven project structure
- Automated browser setup and teardown
- ExtentReports HTML reporting
- Failure screenshot capture using TestNG Listener
- Reusable utility classes
- TestNG XML suite configuration

## Project Structure

```text
src
├── main
│   └── java
│
└── test
    ├── java
    │   ├── base
    │   │   └── BaseTest.java
    │   ├── listeners
    │   │   └── TestListener.java
    │   ├── pages
    │   │   └── LoginPage.java
    │   ├── tests
    │   │   └── LoginTest.java
    │   └── utilities
    │       ├── ExtentManager.java
    │       └── ScreenshotUtil.java
    │
    └── resources
        └── testng.xml
