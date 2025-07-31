
# 🧪 TDD & BDD Final Project — Product Catalog Microservice

This repository contains the **Test-Driven Development (TDD)** and **Behavior-Driven Development (BDD)** final project for the IBM course _"Introduction to Test and Behavior Driven Development"_ on Coursera.

The application is a Python-based microservice that supports a RESTful product catalog. While the base application code was provided, this project focuses on implementing **automated tests**, **API development**, and **BDD scenarios** to ensure robust functionality and UI behavior.

---

## ✅ Project Objectives

Over the course of this project, I completed the following:

### 🧪 Test-Driven Development (TDD)
- Wrote unit tests for:
  - Product model: CRUD operations and search/filter by attributes
  - REST API endpoints: Create, Read, Update, Delete, List, and Search
- Implemented and validated each API endpoint by following the red-green-refactor cycle
- Achieved and maintained:
  - **97% code coverage**
  - **Pylint score of 10.00/10**
  - **Zero flake8 linting errors**

### 🤖 Behavior-Driven Development (BDD)
- Created Gherkin scenarios to test UI behavior
- Implemented step definitions in Python using **Behave** and **Selenium**
- Automated tests for:
  - Viewing, searching, updating, deleting, and listing products via the admin UI
- Populated test data dynamically from `background` tables in `.feature` files

---

## 🛠️ Technologies Used

- **Python 3 / Flask**
- **SQLAlchemy** (ORM for the Product model)
- **Nose** (unit test runner)
- **Flake8** & **Pylint** (linting)
- **Behave** (BDD framework)
- **Selenium** (UI automation)
- **Docker** / **Honcho** / Cloud IDE (provided by IBM)

---

---

## 📁 Project Structure

```
.
├── service/
│   ├── models.py                # Product model with SQLAlchemy
│   ├── routes.py                # RESTful API routes (CRUD + search)
│   ├── config.py, status.py     # App config and status codes
│   ├── common/                  # CLI commands, log & error handlers
├── tests/
│   ├── test_models.py           # TDD unit tests for models
│   ├── test_routes.py           # TDD unit tests for API routes
│   └── factories.py             # Product factory using Faker
├── features/
│   ├── products.feature         # BDD scenarios for UI behavior
│   └── steps/
│       ├── web_steps.py         # UI step definitions using Selenium
│       └── load_steps.py        # Loads background data before scenarios
├── Dockerfile                   # Used to containerize the app
├── requirements.txt             # Project dependencies
└── README.md                    # You are here ✅
```

---

## 📊 Test Results 📷 Screenshots
### Exercise 2: Product Model Testing

**nosetests && make lint Output**

<img width="652" height="266" alt="make lint for Exercise 2" src="https://github.com/user-attachments/assets/7627e654-6048-4162-ad98-11f34e46dbcf" />

* Ater Complting The Tasks:
  
<img width="862" height="561" alt="Excercise 2 Completed  nosetests and make lint" src="https://github.com/user-attachments/assets/c2668e94-6601-4bc6-93e4-f9724dd64ce4" />

### Exercise 3: REST APIs

**nosetests && make lint Output**

<img width="904" height="566" alt="Excercise 3 Completed TDD" src="https://github.com/user-attachments/assets/7b759255-8931-4cc0-ba6a-51154ed94a15" />

### Exercise 6: After Writing BDD Step Definitions

<img width="930" height="422" alt="Excercise 6 BDD all scenarios exist and pass" src="https://github.com/user-attachments/assets/b81677c4-6dd5-41c8-9d5b-88d38d23266a" />

---

## 🧠 What I Learned

- Practiced **Test-Driven Development**: writing failing tests before implementation
- Built and validated **RESTful APIs** from unit tests
- Used **Behavior-Driven Development** to automate browser-based testing
- Applied structured development workflows used in real-world microservice projects
- Interpreted and implemented BDD Gherkin features into testable steps

---

## 🏁 Final Notes

This project was completed as part of the **IBM/CognitiveClass "Introduction to TDD and BDD" course on Coursera**.  
All TDD and BDD code (All testing logic, test data factories, APIs, scenarios, and steps) was implemented by me.  
The core application code (the original Flask microservice) was provided as a scaffold for testing practice.
