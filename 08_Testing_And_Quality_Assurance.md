# 08. Testing & Quality Assurance

---

## What is Software Testing?

Software testing is the process of verifying that software meets requirements and works as intended. It uncovers defects, ensures quality, and builds confidence in software releases. Quality Assurance (QA) covers not just testing but all activities that improve software quality.

---

## Types of Testing

- **Unit Testing:** Test individual functions or methods.
- **Integration Testing:** Test combined parts (modules, services).
- **System Testing:** Test the complete integrated system.
- **Acceptance Testing:** Validate with stakeholders/end users.
- **Regression Testing:** Ensure new changes don’t break old functionality.
- **Performance Testing:** Assess speed, scalability, and stability.
- **Security Testing:** Detect vulnerabilities.
- **Usability Testing:** Check user experience.

---

## Manual vs. Automated Testing

- **Manual Testing:** Human testers execute test cases.
- **Automated Testing:** Scripts validate software automatically (faster, repeatable).

---

## Test Automation Tools

- **Unit:** JUnit (Java), pytest (Python), unittest (Python), Mocha (JavaScript)
- **UI:** Selenium, Cypress
- **API:** Postman, REST-assured

---

## Test-Driven Development (TDD)

- Write failing tests before writing code.
- Develop just enough code to pass the test.
- Refactor and repeat.
- Benefits: fewer bugs, better design, fast feedback.

---

## Continuous Integration (CI)

- Automatically build and test code in response to changes.
- Tools: Jenkins, GitHub Actions, Travis CI, CircleCI.
- Early bug detection, smoother releases.

---

## Code Coverage

- Measures percentage of code exercised by tests.
- Tools: coverage.py, Istanbul, JaCoCo.
- High coverage is good, but don’t write tests just for coverage numbers—focus on important paths.

---

## QA Activities Beyond Testing

- **Static Analysis:** Linting, code style, complexity, security checks.
- **Code Reviews:** Peer review for quality and maintainability.
- **Process Audits:** Ensure adherence to standards.

---

## Best Practices

- Automate as much as possible.
- Write clear, reproducible bug reports.
- Prioritize testing critical and high-risk areas.
- Keep tests, code, and documentation in sync.
- Review test results regularly and act on failures.

---

## Metrics

- **Defect Density:** Bugs per lines of code.
- **Test Pass Rate:** % of tests that pass.
- **Mean Time to Detect/Fix:** How quickly issues are found and resolved.

---

## Interview Questions

1. What is the difference between unit and integration testing?
2. How does TDD improve software quality?
3. What is code coverage and why is it important?
4. How do you automate a regression test suite?
5. What’s the role of QA in agile development?

---

## References

- [ISTQB Glossary](https://glossary.istqb.org/en/search)
- [pytest Documentation](https://docs.pytest.org/en/stable/)
- [SeleniumHQ](https://www.selenium.dev/)

---

## Exercises

1. Write unit tests for a function using pytest or JUnit.
2. Set up a CI pipeline to run tests on every push.
3. Automate a simple browser scenario with Selenium.
4. Define acceptance criteria for a user story.
5. Analyze a failed test and debug the issue.

---

## Summary

Testing and QA are essential for reliable software. They reduce risk, improve quality, and ensure customer satisfaction. A strong testing mindset is a hallmark of a professional software engineer.

---
