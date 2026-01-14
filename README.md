# Hybrid-to-BDD-Framework

A simple **Hybrid BDD automation framework** built using **Java, Selenium, Cucumber, and TestNG**.
This project demonstrates how to write readable BDD tests while keeping a structured automation framework.

---

## 📌 What This Project Does

* Uses **Cucumber (BDD)** for writing test scenarios in plain English
* Uses **Selenium WebDriver** for browser automation
* Uses **TestNG** for test execution
* Follows a hybrid framework structure for better organization and reuse

---

## 🛠️ Tools & Technologies

* Java
* Maven
* Selenium WebDriver
* Cucumber
* TestNG

---

## 📁 Project Structure

```
Hybrid-to-BDD-Framework/
├── src/                 # Step definitions, hooks, utilities
├── features/            # Cucumber feature files
├── pom.xml              # Maven dependencies
├── testng.xml           # TestNG suite
├── target/              # Build output
└── README.md            # Project documentation
```

---

## 🚀 How to Run the Tests

### Prerequisites

* Java (JDK 8 or higher)
* Maven
* IDE (IntelliJ or Eclipse)
* Chrome / Firefox browser

---

### Steps

1. **Clone the repository**

   ```bash
   git clone https://github.com/qa-julienne/Hybrid-to-BDD-Framework.git
   ```

2. **Go to the project folder**

   ```bash
   cd Hybrid-to-BDD-Framework
   ```

3. **Run tests**

   ```bash
   mvn test
   ```

Or run using TestNG:

```bash
mvn test -DsuiteXmlFile=testng.xml
```

---

## 📝 Writing Tests

### Feature File Example

```gherkin
Feature: Login

  Scenario: Valid user login
    Given user is on login page
    When user enters valid credentials
    Then user should be logged in
```

### Step Definition Example

```java
@Given("user is on login page")
public void userOnLoginPage() {
    // Selenium code
}
```

---

## 📊 Reports

After execution, test reports are generated in:

* `target`
* `test-output`

