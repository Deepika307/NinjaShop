# NinjaShop Automation Framework

##  Project Overview

NinjaShop is a Selenium-Java Automation Test Framework developed to automate end-to-end testing of a demo e-commerce application:
-> https://tutorialsninja.com/demo

The framework is designed using the **Page Object Model (POM)** pattern and follows industry best practices like reusable components, data-driven testing, and structured reporting.

---
## Project Structure
```
NinjaShop/
│
├── src/
│   ├── main/java/com/srm/ninjashop/
│   │   ├── config/
│   │   │   └── ConfigReader.java
│   │   │
│   │   ├── driver/
│   │   │   └── DriverFactory.java
│   │   │
│   │   ├── listeners/
│   │   │   └── TestListener.java
│   │   │
│   │   ├── pages/
│   │   │   ├── BasePage.java
│   │   │   ├── HomePage.java
│   │   │   ├── LoginPage.java
│   │   │   ├── RegisterPage.java
│   │   │   ├── AccountPage.java
│   │   │   ├── ProductPage.java
│   │   │   ├── CategoryPage.java
│   │   │   ├── SearchPage.java
│   │   │   ├── CartPage.java
│   │   │   ├── CheckoutPage.java
│   │   │   └── CheckoutSuccessPage.java
│   │   │
│   │   └── utils/
│   │       ├── ExtentReportManager.java
│   │       └── ScreenshotUtils.java
│   │
│   ├── test/java/com/srm/ninjashop/
│   │   ├── tests/
│   │   │   ├── LoginTest.java
│   │   │   ├── RegisterTest.java
│   │   │   ├── ProductTest.java
│   │   │   ├── CartTest.java
│   │   │   ├── CheckoutTest.java
│   │   │   └── ValidationTest.java
│
├── testng.xml
├── pom.xml
├── config.properties
├── screenshots/
└── README.md
```
##  Objectives

* Automate key e-commerce workflows
* Implement scalable test framework using POM
* Ensure maintainability and reusability
* Generate detailed execution reports
* Capture screenshots on test failure

---

##  Test Coverage

###  Authentication

* Login with valid credentials
* Login with invalid credentials
* User registration
* Logout functionality

###  Product Module

* Search product by keyword
* Category navigation
* Product detail validation

###  Cart Module

* Add product to cart
* Update quantity
* Remove product
* Validate cart total

###  Checkout Module

* Proceed to checkout
* Enter delivery details
* Confirm order
* Validate order success

###  Form Validations

* Empty field validation
* Invalid email validation
* Checkout form validation

---

##  Framework Design

###  Page Object Model (POM)

* Each page has a dedicated class
* Locators and actions are encapsulated
* Test classes interact only with page methods

###  Key Components

* `BasePage` → Common reusable methods
* `DriverFactory` → WebDriver initialization
* `ConfigReader` → Reads config.properties
* `TestListener` → Screenshot on failure
* `ExtentReportManager` → HTML reporting

---

##  Tech Stack

* Java
* Selenium WebDriver
* TestNG
* Maven
* WebDriverManager
* ExtentReports

---

##  Configuration

Located in:

```
config.properties
```

Includes:

* Browser (chrome/firefox)
* Base URL
* Timeout

---

## ▶️ How to Run the Project

### ▶️ Run Tests

 run via TestNG:

* Right-click `testng.xml` → Run

---

## 📊 Reporting

* Extent Reports generated after execution
* Includes:

  * Test status (Pass/Fail)
  * Error logs
  * Screenshot on failure

---

## 📸 Screenshots

* Captured automatically on test failure
* Stored in `/screenshots` folder with timestamp

---

## ✅ Key Features

✔ Page Object Model (POM)
✔ Data-driven testing using TestNG
✔ Config-based execution (no hardcoding)
✔ Explicit waits (no Thread.sleep)
✔ Screenshot on failure
✔ Extent HTML reports

---

## 🚀 Future Enhancements

* Parallel execution
* Excel/JSON DataProvider
* Retry failed tests
* Headless browser execution

---

## 👩‍💻 Author

**Deepika Kantheti**



---
