# 03. Requirements Engineering

---

## What is Requirements Engineering?

Requirements engineering is the discipline of identifying, documenting, analyzing, prioritizing, and maintaining the requirements for a software system. It ensures that the software meets the actual needs of users and stakeholders and is a critical phase in the Software Development Life Cycle (SDLC).

---

## Why is Requirements Engineering Important?

- **Foundation for Success:** Clear requirements prevent misunderstandings and rework.
- **Stakeholder Satisfaction:** Ensures the final product aligns with user needs.
- **Scope Management:** Defines boundaries and helps avoid scope creep.
- **Basis for Design, Testing, and Validation:** Requirements guide architecture and test cases.

---

## Types of Requirements

- **Functional Requirements:** Describe what the system should do (features, behaviors, services).
    - Example: "The system shall allow users to reset their password via email."
- **Non-Functional Requirements:** Specify how the system performs a function (quality attributes).
    - Examples: performance, reliability, scalability, usability, security.
    - Example: "The system shall respond to user queries within two seconds."
- **Domain Requirements:** Constraints imposed by the domain or business.
    - Example: "Invoices must comply with local tax regulations."

---

## Requirements Engineering Process

1. **Requirements Elicitation**
    - Collecting requirements from users, stakeholders, and domain experts.
    - Techniques: interviews, surveys, observation, brainstorming, workshops, prototyping.

2. **Requirements Analysis**
    - Clarifying, prioritizing, and resolving conflicts in requirements.
    - Identifying ambiguities, inconsistencies, and feasibility.

3. **Requirements Specification**
    - Creating a clear, complete, and verifiable documentation of requirements.
    - Use of SRS (Software Requirements Specification) documents, user stories, use cases.

4. **Requirements Validation**
    - Ensuring requirements are correct, complete, and agreed upon.
    - Methods: reviews, walkthroughs, prototyping, test-case generation.

5. **Requirements Management**
    - Tracking requirements changes, versioning, and traceability throughout the project.

---

## Elicitation Techniques (Detailed)

- **Interviews:** Direct discussions with stakeholders.
- **Questionnaires/Surveys:** Collect data from many users quickly.
- **Observation:** Watch users interact with current systems.
- **Workshops:** Group meetings for collaborative requirement discovery.
- **Prototyping:** Create mockups to clarify requirements.
- **Document Analysis:** Study existing documentation for legacy systems.
- **Use Cases/User Stories:** Describe interactions between users and the system.

---

## Writing Good Requirements

- **Clear:** No ambiguity or vagueness.
- **Complete:** Covers all necessary aspects.
- **Consistent:** No conflicts between requirements.
- **Verifiable:** Can be checked by tests or inspection.
- **Feasible:** Can be implemented within constraints.
- **Traceable:** Each requirement can be tracked through design, coding, and testing.

---

## Example: User Story vs. SRS

**User Story:**
```
As a customer, I want to receive an email confirmation after placing an order so that I can verify my purchase.
```

**SRS Statement:**
```
3.2.1 The system shall send an order confirmation email to the customer immediately after a successful order placement.
```

---

## Requirements Prioritization

- **MoSCoW Method:** Must have, Should have, Could have, Won't have.
- **Kano Model:** Categorizes features into basic, performance, and excitement.
- **100-Dollar Test:** Stakeholders distribute a budget among features.

---

## Tools for Requirements Engineering

- **Jira, Confluence**
- **IBM DOORS**
- **Atlassian Trello**
- **ReqIF**
- **Enterprise Architect**

---

## Common Challenges

- **Changing Requirements:** Stakeholder needs evolve over time.
- **Ambiguity:** Poorly defined or vague requirements.
- **Incomplete Requirements:** Missing details or scenarios.
- **Conflicting Requirements:** Different stakeholders want different things.
- **Traceability:** Difficulty tracking requirements through design, code, and tests.

---

## Requirements Traceability Matrix (RTM)

A tool to map and track requirements from origin to delivery. Ensures all requirements are addressed in design, implementation, and testing.

| Requirement ID | Description | Design Module | Test Case ID |
|----------------|-------------|--------------|-------------|
| FR-001         | User Login  | Auth Module  | TC-01, TC-02|

---

## Best Practices

- Involve all relevant stakeholders from the beginning.
- Use visual aids (mockups, diagrams).
- Regularly review and update requirements.
- Prioritize requirements based on value and risk.
- Maintain a change log for requirements updates.

---

## Interview Questions

1. What are functional vs. non-functional requirements?
2. How do you gather requirements for a new system?
3. What are common pitfalls in requirements engineering?
4. Explain requirements traceability and its importance.
5. Describe a situation when you had to resolve conflicting requirements.

---

## References

- [IEEE 830-1998 - SRS Standard](https://en.wikipedia.org/wiki/Software_requirements_specification)
- [Atlassian: Requirements](https://www.atlassian.com/software-development/requirements)
- [BABOK Guide](https://www.iiba.org/standards-and-resources/babok/)

---

## Exercises

1. Draft a user story and an SRS statement for the same feature.
2. Create a mini RTM for a login feature.
3. Conduct a mock requirements elicitation interview for an e-commerce checkout system.
4. List three non-functional requirements for a banking application and explain why they are important.
5. Identify potential conflicts in requirements for a social media platform and propose resolutions.

---

## Summary

Requirements engineering is the backbone of successful software projects. Well-managed requirements reduce risk, drive design and testing, and ensure the final product delivers value to stakeholders.

---
