# Day 3 - Data Modeling in Salesforce

## 1. Difference Between App, Object, Record, and Field

### App
An App in Salesforce is a collection of related tools, tabs, and objects used for a specific business process.

**Example:**  
Sales App or College Management App

---

### Object
An Object is like a database table that stores similar types of data.

**Example:**  
Student Object

---

### Record
A Record is a single entry inside an object.

**Example:**  
One student’s information such as Rahul Kumar

---

### Field
A Field is a single piece of information inside a record.

**Example:**  
Student Name, Roll Number, or Email

---

## Simple Example

- **App** → College Management App  
- **Object** → Student  
- **Record** → Rahul Kumar  
- **Field** → Roll Number  

---

# 2. Standard vs Custom Objects

## Standard Objects
Standard Objects are already provided by Salesforce for common business needs.

### Features
- Pre-built by Salesforce
- Used in most business applications
- Cannot be removed easily

### Examples
- Account
- Contact
- Opportunity

---

## Custom Objects
Custom Objects are created by users based on company requirements.

### Features
- Fully customizable
- Used for specific business needs
- Created manually by developers or admins

### Examples
- Student__c
- Course__c
- Library__c

---

# 3. Your College Data Model

## Objects

- Student
- Course
- Faculty
- Department

---

## Relationships

- A Student enrolls in a Course
- A Faculty teaches a Course
- A Department contains many Faculty members

---

## Diagram

```text
Department
    |
    | contains
    v
Faculty ---- teaches ----> Course
                                ^
                                |
                          enrolled by
                                |
                             Student
```

---

# 4. Formula Fields

## Formula Field 1 – Student Full Name

### Formula

```text
First_Name + " " + Last_Name
```

### Explanation
This formula automatically combines the first name and last name of a student.

---

## Formula Field 2 – Remaining Seats

### Formula

```text
Total_Seats - Filled_Seats
```

### Explanation
This formula calculates the number of seats still available in a course.

---

## Formula Field 3 – Student Age

### Formula

```text
TODAY() - Date_of_Birth
```

### Explanation
This formula calculates the student’s age automatically using the date of birth.

---

# 5. Validation Rules

## Rule 1 – Email Cannot Be Empty

### Validation Rule

```text
Email field should not be blank
```

### Problem Prevented
This prevents storing incomplete contact information.

---

## Rule 2 – Student Age Cannot Be Negative

### Validation Rule

```text
Age >= 0
```

### Problem Prevented
This prevents invalid age values from being entered into the system.

---

## Rule 3 – Course Seats Cannot Exceed Limit

### Validation Rule

```text
Filled_Seats <= Total_Seats
```

### Problem Prevented
This prevents enrolling more students than the available course seats.

---

# 6. Reflection

## Why Structured Enterprise Data Matters

Structured enterprise data is important because it keeps information organized, accurate, and easy to manage. Random spreadsheets often contain duplicate data, missing values, and mistakes.

In a structured data model, companies can easily search records, generate reports, and make better decisions. For example, in a college management system, structured data helps manage students, courses, faculty, and departments properly.

Relationships between objects make it easier to track which student enrolled in which course and which faculty teaches that course.

Validation rules and formula fields improve data quality by reducing manual errors. Overall, structured enterprise data improves efficiency, saves time, and helps organizations grow smoothly.

---

