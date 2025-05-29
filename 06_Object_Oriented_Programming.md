# 06. Object-Oriented Programming & Principles (OOP)

---

## What is Object-Oriented Programming (OOP)?

OOP is a programming paradigm based on the concept of "objects"—data structures encapsulating data and behaviors. It models real-world entities, relationships, and operations, leading to code that is modular, reusable, and maintainable.

---

## Four Main Principles

### 1. Encapsulation

- Bundles data (attributes) and related behaviors (methods) into a single unit (class).
- Hides internal state; only exposes what’s necessary via public interfaces.
- Example:
    ```python
    class User:
        def __init__(self, name):
            self.__name = name  # private attribute
        def get_name(self):
            return self.__name
    ```

### 2. Abstraction

- Exposes only essential features and hides unnecessary details.
- Achieved via abstract classes and interfaces.
- Example: A car exposes "drive" and "brake," not engine mechanics.

### 3. Inheritance

- Allows a new class to inherit properties and methods from an existing class.
- Promotes reusability and hierarchical relationships.
- Example:
    ```python
    class Animal:
        def speak(self):
            pass
    class Dog(Animal):
        def speak(self):
            return "Woof!"
    ```

### 4. Polymorphism

- Enables one interface to be used for different data types.
- Achieved via method overriding and overloading.
- Example:
    ```python
    animals = [Dog(), Cat()]
    for animal in animals:
        print(animal.speak())  # Each animal speaks differently
    ```

---

## OOP in Practice

- **Class:** Blueprint for creating objects.
- **Object:** Instance of a class.
- **Method:** Function associated with an object.
- **Attribute:** Variable associated with an object.

---

## Access Modifiers

- **Public:** Accessible from anywhere.
- **Protected:** Accessible within class and subclasses.
- **Private:** Accessible only within the class.

---

## OOP & SOLID

- OOP is most effective when combined with SOLID principles.
- Promotes high cohesion and low coupling.

---

## Benefits of OOP

- **Modularity:** Code is organized into discrete classes.
- **Reusability:** Inheritance and composition.
- **Maintainability:** Changes in one class minimally affect others.
- **Extensibility:** Easy to add new behaviors.

---

## OOP Design Patterns

- Many design patterns (Factory, Singleton, Observer) leverage OOP principles.

---

## Pitfalls to Avoid

- **God Object:** One class does too much.
- **Deep Inheritance:** Prefer composition to deep hierarchies.
- **Leaky Abstractions:** Exposing internal details.
- **Overuse of Inheritance:** Can reduce flexibility.

---

## Interview Questions

1. Explain encapsulation with an example.
2. How does polymorphism work in OOP?
3. What is the difference between an abstract class and an interface?
4. When would you use inheritance vs. composition?
5. Describe a scenario where OOP improved code maintainability.

---

## References

- [Wikipedia: Object-Oriented Programming](https://en.wikipedia.org/wiki/Object-oriented_programming)
- [Python OOP Documentation](https://docs.python.org/3/tutorial/classes.html)
- [SOLID Principles](https://en.wikipedia.org/wiki/SOLID)

---

## Exercises

1. Write a class hierarchy for vehicles (Car, Bike, Truck) with common and unique behaviors.
2. Implement method overriding and demonstrate polymorphism.
3. Refactor a procedural code segment into an OOP design.
4. Explain how encapsulation helps with debugging and testing.
5. Design an interface for a payment processing system.

---

## Summary

OOP is a cornerstone of modern software engineering. Mastering its principles leads to more robust, scalable, and maintainable systems—qualities highly valued in interviews and on the job.

---
