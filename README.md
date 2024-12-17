
# Vehicle Details Test Automation Project

This project automates the testing of vehicle details validation on the Motors.co.uk platform using Selenium WebDriver and TestNG. 
The project follows the **Page Object Model (POM)** design pattern for better maintainability and reusability.

---

## Project Overview

### Key Features:
- Test vehicle details with partial and complete form inputs.
- Validation of registration, mileage, and postcode fields.
- Modular Page Object Model to keep test logic and page-specific actions separate.

---

## Prerequisites

Ensure the following tools and dependencies are installed on your system:

1. **Java Development Kit (JDK)** - Version 8 or above  
   [Download JDK](https://www.oracle.com/java/technologies/javase-jdk11-downloads.html)
2. **Maven** - For managing dependencies and building the project  
   [Download Maven](https://maven.apache.org/)
3. **IntelliJ IDEA** (or any preferred IDE)  
   [Download IntelliJ IDEA](https://www.jetbrains.com/idea/)
4. **Google Chrome** - The browser used for testing.

---


## Setup Instructions

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/am-rabiu/vehicle-check
   cd vehicle-check
   ```

2. **Install Dependencies**:
   Use Maven to download project dependencies.
   ```bash
   mvn clean install
   ```


## Running the Tests

To execute the test cases, run the following command from the project root:

```bash
mvn test
```

Alternatively, run `VehicleDetailsTests.java` directly from your IDE.

---

## Reports

- TestNG generates an HTML report after test execution.
- The report is saved in the `test-output` directory:
  ```plaintext
  target\surefire-reports\index.html
  ```

---

## Key Classes

1. **WebDriverHelper**:
   - Manages WebDriver setup, initialization, and utility functions like handling cookies.

2. **VehicleDetailsPage**:
   - Contains page-specific actions like entering registration, mileage, and postcode.

3. **VehicleDetailsTests**:
   - Contains test methods:
     - `getVehicleDetailsWithOnlyRegistrationFieldFilled`
     - `getVehicleDetailsWithAllFormFieldsFilled`

---

## Future Enhancements

- Add ExtentReports for better reporting.
- Integrate with CI/CD tools like Jenkins.
- Add support for other browsers using a config file to set any installed browser.

---



