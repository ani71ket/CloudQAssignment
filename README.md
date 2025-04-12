# Selenium-Based Automated Form Field Testing in C#

## Overview
This project demonstrates how to build a robust automated testing solution in C# using Selenium WebDriver. The primary objective is to validate key input fields within a web application form, ensuring they function correctly even when the DOM structure or styling changes over time.

## Objective
Develop a C# application utilizing Selenium to verify the functionality of three specific input fields on a web form. The test should remain stable regardless of changes to the layout, positioning, or styling of the HTML elements being tested.

## Testing Strategy
The automation script is designed to interact with the form hosted at:
`https://app.cloudqa.io/home/AutomationPracticeForm`

The targeted fields include:
- First Name
- Last Name
- Mobile Number

Each field is located dynamically using its `name` attribute, which ensures the script remains resilient to UI modifications. 

### Steps Performed:
1. Initialize the Chrome WebDriver using the `Selenium.Chrome` package.
2. Navigate to the form URL.
3. Locate each form field based on its `name` attribute.
4. Input test data into each field.
5. Retrieve the current value of each input element.
6. Compare the entered value against the expected input.
7. Log the test result (pass/fail) based on the match outcome.

This method allows the test to maintain reliability without relying on hardcoded element positions, making it suitable for regression testing and continuous integration.

## Tools & Technologies
- **Programming Language:** C#
- **Testing Framework:** Selenium WebDriver
- **Browser Driver:** ChromeDriver
- **Target Platform:** Web-based form UI

## Conclusion
This project showcases a simple yet effective way to automate and verify form input fields using Selenium in C#. By targeting attributes like `name` instead of relying on CSS or XPath selectors, the tests are resilient to structural changes in the DOM, providing a maintainable approach for future scalability and updates.
