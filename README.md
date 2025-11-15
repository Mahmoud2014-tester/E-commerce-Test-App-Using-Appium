## E-commerce Test App – Mobile Automation Testing (Appium + Java)
This repository contains automated mobile test cases for an E-commerce Android Application using **Appium, Java, and Eclipse IDE.**
The project demonstrates real-world mobile automation practices including form submission, toast message validation, scrolling, cart validation, and hybrid app browser testing.

## Project Overview
The goal of this project is to automate key user flows in the E-commerce Android App, ensuring that core functionalities work as expected.
The tests cover:
**1- Filling forms on the onboarding page**
**2- Capturing and asserting Toast messages**
**3- Scrolling through lists and adding products to cart**
**4- Validating cart items using assertions**
**5- Handling Hybrid App flows using external browser redirection**

## Tech Stack
```
| Component                     | Details                                       |
| ----------------------------- | --------------------------------------------- |
| **Automation Tool**           | Appium                                        |
| **Programming Language**      | Java                                          |
| **IDE**                       | Eclipse                                       |
| **Build Tool**                | Maven                                         |
| **Android Automation Engine** | UiAutomator2                                  |

```

```
E-commerce-Test-App-Using-Appium/
│
├── src/
│   ├── main/java/
│   │   ├── e_commerceProject  -> App.java
│   │
│   └── test/java/
│       ├── e_commerceProject          -> BaseTest.java
|                                      -> ConvertFromNativeToHybridApp.java
|                                      -> FirstTestCase.java
|                                      -> HandleToastMessage.java
|                                      -> ScrollToElementAndAddToCart.java
│
├── resources/
│   ├── app/                -> General-Store.apk
│
├── pom.xml                 -> Maven dependencies
├── README.md

```

## Device Capabilities Setup
UiAutomator2Options configuration:

```
UiAutomator2Options options = new UiAutomator2Options();
options.setDeviceName("Saber");
options.setPlatformName("Android");
options.setApp("path/to/General-Store.apk");
options.setAutomationName("UiAutomator2");
```

## Framework Features
```
1- Page Object Model (POM)
2- Centralized driver handling
3- Reusable utilities (scroll, tap, waits)
4- Toast message handling utilities
5- Dynamic element locating
6- Cross-screen navigation support
7- Mobile gestures if included
```
