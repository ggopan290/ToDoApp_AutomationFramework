# AutomationFramework_Gopika

## 📌 Overview

`AutomationFramework_Gopika` is a Maven-based test automation framework developed using:
- **Java**
- **Selenium WebDriver**
- **Cucumber (BDD)**
- **JUnit**
- **Extent Reports**

It automates UI tests for a React-based ToDo application with a Node.js/Express backend.

---

## 🎯 Objectives

- Validate login functionality.
- Validate ToDo dashboard operations: adding, editing, deleting tasks.
- Generate comprehensive reports with screenshots.
- Maintain modular, scalable code using industry-standard practices.

---

## 🧩 Tech Stack

| Layer         | Technology                        |
|--------------|-----------------------------------|
| Language      | Java                              |
| Automation    | Selenium WebDriver, Cucumber BDD  |
| Test Runner   | JUnit                             |
| Build Tool    | Maven                             |
| Reports       | ExtentReports                     |
| Frontend App  | React.js                          |
| Backend API   | Express.js (Node.js)              |

---

## 📁 Project Structure

```
AutomationFramework_Gopika/
│
├── src/
│   ├── main/java/utilities/       # WebDriver, Screenshot, Report Utils
│   ├── test/java/
│   │   ├── runners/               # Test runner class
│   │   ├── stepDefinitions/       # Step definition files
│   ├── test/resources/features/   # Cucumber feature files
│
├── Automation Reports/
│   ├── screenshots/               # Screenshot on failure/success
│   └── Automation-Report-*.html   # Extent HTML reports
│
├── ToDoApp/
│   ├── client/                    # React frontend
│   └── server/                    # Express backend
│
└── pom.xml                        # Maven configuration
```

---

## 🚀 How to Run Tests

### 1. Clone and Install

```bash
git clone <repo-url>
cd AutomationFramework_Gopika
npm install --prefix ToDoApp/server
npm install --prefix ToDoApp/client
```

### 2. Start Backend and Frontend

```bash
# Start Node server
cd ToDoApp/server
node server.js

# In a new terminal: start React frontend
cd ../client
npm start
```

### 3. Execute UI Tests

```bash
mvn clean test
```

Extent report and screenshots will be generated in `Automation Reports/`.

---

## 🧪 Features Covered

- ✅ Login validation with alert handling.
- ✅ Add a new ToDo item.
- ✅ Edit an existing item.
- ✅ Delete an item.
- ✅ Auto-screenshot on failure/success.
- ✅ Extent HTML report after each run.

---

## 📌 Notes

- Runs against a **local Node.js server** on `http://localhost:4000`.
- Report and screenshot folders are cleared on every test execution.
- Step-wise screenshots for passed and failed steps.

---

## 📞 Contact

For issues or contributions, please reach out to the project maintainer or open an issue in the repo.

---