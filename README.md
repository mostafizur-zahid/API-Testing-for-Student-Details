<div align="center">

# 🚀 API Testing for Student Details

### Professional REST API Automation Testing Framework using Postman & Newman

![Postman](https://img.shields.io/badge/Postman-API_Testing-orange?style=for-the-badge&logo=postman)
![Newman](https://img.shields.io/badge/Newman-Automation-blue?style=for-the-badge)
![JavaScript](https://img.shields.io/badge/JavaScript-Test_Scripting-yellow?style=for-the-badge&logo=javascript)
![REST API](https://img.shields.io/badge/REST_API-Testing-success?style=for-the-badge)
![Status](https://img.shields.io/badge/Project-Completed-brightgreen?style=for-the-badge)
[![Live Report](https://img.shields.io/badge/Newman-Live_Report-success?style=for-the-badge)](https://mostafizur-zahid.github.io/API-Testing-for-Student-Details/report.html)

---

### 🔥 Complete End-to-End CRUD API Automation Testing Project

</div>

---

# 📌 Project Overview

This repository contains a complete **REST API Automation Testing Framework** developed for testing Student Details APIs using:

- ✅ Postman
- ✅ Newman
- ✅ JavaScript Assertions
- ✅ Dynamic Variables
- ✅ Environment Variables
- ✅ Automated HTML Reporting
- ✅ API Chaining
- ✅ Runtime Data Injection

The project simulates real-world API automation workflows by validating complete CRUD operations and generating professional execution reports.

---

# 🌐 API Base URL

```text
https://thetestingworldapi.com/api
```

---

# 🧪 Technologies Used

| Technology | Purpose |
|---|---|
| Postman | API Testing & Automation |
| Newman | Collection Execution |
| Newman HTML Extra | HTML Dashboard Reporting |
| JavaScript | Assertions & Runtime Scripting |
| JSON | Request & Response Handling |
| GitHub Pages | Live Report Hosting |
| GitHub | Version Control & Portfolio |

---

# 🏗️ Framework Architecture

```text
Postman Collection
        ↓
Dynamic Variables
        ↓
Environment Variables
        ↓
API Chaining
        ↓
Assertions & Validations
        ↓
Newman CLI Execution
        ↓
HTML Dashboard Report
        ↓
GitHub Pages Hosting
```

---

# 📂 Repository Structure

```bash
API-Testing-for-Student-Details/
│
├── Collection/
│   └── Rest_API_Testing_For_Student_Details.postman_collection.json
│
├── Environment/
│   └── StudentDetails.postman_environment.json
│
├── newman/
│   └── Rest_API_Testing_For_Student_Details.html
│
├── assets/
│   └── newman-dashboard.png
│
├── Newman Summary Report.pdf
│
├── report.html
│
└── README.md
```

---

# 🔥 Complete API Workflow

The framework executes a complete end-to-end student lifecycle workflow.

```text
Get Student List
        ↓
Create Student
        ↓
Get Specific Student
        ↓
Update Student
        ↓
Create Technical Skills
        ↓
Create Student Address
        ↓
Get Final Student Details
        ↓
Delete Student
        ↓
Verify Student Deletion
```

---

# 🚀 API Modules

---

# ✅ 1. Get Student List

Retrieves all available student records from the server.

## Validations

- Status code validation
- Response time validation
- Response size validation
- JSON response validation

---

# ✅ 2. Create Student

Creates a new student dynamically using runtime-generated data.

## Dynamic Data Used

- Random first name
- Random middle name
- Random last name
- Dynamic date of birth

---

## 🔥 Dynamic Variable Script

```javascript
var first_name = pm.variables.replaceIn('{{$randomNamePrefix}}');
pm.environment.set("first_name", first_name);

var middle_name = pm.variables.replaceIn('{{$randomFirstName}}');
pm.environment.set("middle_name", middle_name);

var last_name = pm.variables.replaceIn('{{$randomLastName}}');
pm.environment.set("last_name", last_name);

var date_of_birth = require('moment')().format('DD-MM-YYYY');
pm.environment.set("date_of_birth", date_of_birth);
```

---

## Example Request Body

```json
{
    "first_name": "{{first_name}}",

    "middle_name": "{{middle_name}}",

    "last_name": "{{last_name}}",

    "date_of_birth": "{{date_of_birth}}"
}
```

---

# ✅ 3. Get Specific Student

Retrieves dynamically created student information using stored student ID.

## Validations

- Status validation
- Response validation
- JSON validation
- Student information verification

---

# ✅ 4. Update Student

Updates existing student information dynamically.

## Features

- Runtime data update
- Variable reuse
- API chaining
- Response verification

---

# ✅ 5. Create Technical Skills

Creates dynamic technical skill information for the student.

## Features

✅ Dynamic Programming Languages  
✅ Random Runtime Data  
✅ Environment Variable Injection  
✅ API Data Linking  

---

## Example Dynamic Skill Script

```javascript
var skills = [
    "Java",
    "Python",
    "C++",
    "JavaScript",
    "Go"
];

var lang1 = skills[Math.floor(Math.random() * skills.length)];
var lang2 = skills[Math.floor(Math.random() * skills.length)];

pm.environment.set("lang1", lang1);
pm.environment.set("lang2", lang2);
```

---

# ✅ 6. Create Student Address

Creates permanent address information dynamically.

## Features

- Dynamic city generation
- Dynamic country generation
- Dynamic phone numbers
- Runtime UUID generation

---

## Example Address Request Body

```json
{
    "Permanent_Address": {

        "House_Number": "{{house_number}}",

        "City": "{{city}}",

        "State": "{{state}}",

        "Country": "{{country}}",

        "PhoneNumber": [

            {
                "Std_Code": "{{std_code1}}",

                "Home": "{{home1}}",

                "Mobile": "{{mobile1}}"
            },

            {
                "Std_Code": "{{std_code2}}",

                "Home": "{{home2}}",

                "Mobile": "{{mobile2}}"
            }
        ]
    },

    "stId": "{{stId}}"
}
```

---

# ✅ 7. Final Student Details Verification

Validates final combined student information after all API operations.

## Verification Includes

- Student creation validation
- Technical skill linking validation
- Address information validation
- Complete workflow verification

---

# ✅ 8. Delete Student

Deletes dynamically created student data.

## Validations

- Delete response validation
- Status code verification
- Resource deletion confirmation

---

# ✅ 9. Verify Student Deletion

Confirms that the deleted student resource no longer exists.

## Features

✅ Negative API Testing  
✅ Resource Validation  
✅ Response Verification  
✅ Workflow Integrity Validation  

---

# 🧠 Dynamic Variables Used

This project heavily uses Postman Dynamic Variables to simulate real-world runtime automation.

| Variable | Purpose |
|---|---|
| `{{$randomFirstName}}` | Random first name |
| `{{$randomLastName}}` | Random surname |
| `{{$randomCity}}` | Dynamic city |
| `{{$randomCountry}}` | Dynamic country |
| `{{$randomPhoneNumber}}` | Random phone number |
| `{{$randomUUID}}` | Unique identifier |
| `{{$randomInt}}` | Random integer |

---

# 🔥 Assertions Implemented

The framework includes comprehensive API validations.

✅ HTTP Status Code Validation  
✅ Response Time Validation  
✅ Response Size Validation  
✅ JSON Validation  
✅ Dynamic Data Matching  
✅ Business Logic Validation  
✅ Delete API Validation  
✅ CRUD Workflow Validation  
✅ Environment Variable Validation  
✅ Negative Testing  

---

# 📌 Example Assertions

## Status Code Validation

```javascript
pm.expect(pm.response.code).to.eql(200);
```

---

## Response Time Validation

```javascript
pm.expect(pm.response.responseTime).to.be.below(3000);
```

---

## JSON Validation

```javascript
pm.response.to.be.json;
```

---

## Dynamic Data Validation

```javascript
pm.expect(pm.environment.get("first_name"))
.to.eql(responseBody.data.first_name);
```

---

# 📊 Newman HTML Dashboard Report

The project generates a professional Newman HTML dashboard report after execution.

---

# 📈 Execution Summary

| Metric | Result |
|---|---|
| Total Requests | 9 |
| Total Assertions | 88 |
| Failed Tests | 2 |
| Skipped Tests | 0 |
| Average Response Time | 199ms |
| Total Run Duration | 2.2s |

---

# 📸 Newman Dashboard Preview

![Newman Dashboard](./assets/newman-dashboard.png)

---

# 🌐 Live Newman HTML Report

## 🔗 View Live Report

### 🚀 https://mostafizur-zahid.github.io/API-Testing-for-Student-Details/report.html

---

# ⚠️ Known Assertion Notes

Two assertions intentionally failed because the API server returned:

```text
200 OK
```

instead of:

```text
201 Created
```

for:

- Create Technical Skills API
- Create Student Address API

This issue originates from the API server implementation itself, not from the automation framework.

---

# ▶️ Run Collection Using Newman

---

# ✅ Install Newman

```bash
npm install -g newman
```

---

# ✅ Install Newman HTML Reporter

```bash
npm install -g newman-reporter-htmlextra
```

---

# ✅ Execute Collection

```bash
newman run Rest_API_Testing_For_Student_Details.postman_collection.json \
-e StudentDetails.postman_environment.json \
-r htmlextra
```

---

# 📁 Environment Variables

Environment variables are used for:

- Runtime data storage
- API chaining
- Dynamic validations
- Reusable execution flow

---

## Example Variables

```text
base_url
id
first_name
middle_name
last_name
date_of_birth
lang1
lang2
city
country
house_number
stId
```

---

# 🎯 Key Learning Outcomes

This project demonstrates practical experience with:

✅ REST API Automation  
✅ CRUD API Testing  
✅ Postman JavaScript Scripting  
✅ Dynamic Variables Handling  
✅ Environment Variable Management  
✅ API Chaining  
✅ Newman CLI Automation  
✅ Automated HTML Reporting  
✅ Runtime Assertions  
✅ Response Validation  
✅ Negative Testing  
✅ Professional API Workflow Design  

---

# 🔥 Project Highlights

✅ Complete End-to-End CRUD API Automation  
✅ Runtime Dynamic Data Generation  
✅ Professional Newman HTML Dashboard  
✅ GitHub Pages Live Reporting  
✅ Environment Variable Chaining  
✅ Portfolio-Ready Project Architecture  
✅ Real-World Automation Workflow  
✅ Advanced Postman Scripting  

---

# 👨‍💻 Author

# Md. Mostafizur Rahman Zahid

🎓 CSE Graduate  
🔐 Aspiring Security Engineer  
🧪 SQA & API Automation Enthusiast  
⚡ Cybersecurity & DevSecOps Learner  
🤖 NLP Researcher  

---

# 🔗 Connect With Me

## LinkedIn

https://www.linkedin.com/in/mostafizur-zahid/

---

## GitHub

https://github.com/mostafizur-zahid

---

# ⭐ Repository

## API Testing for Student Details

https://github.com/mostafizur-zahid/API-Testing-for-Student-Details

---

<div align="center">

### 🌟 If you found this project helpful, consider giving it a star on GitHub.

</div>
