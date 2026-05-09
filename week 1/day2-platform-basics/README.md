# Salesforce Platform Basics

## 1. What is Salesforce Platform?

Salesforce Platform is a cloud-based platform that helps businesses build applications, manage customer relationships, automate workflows, and store data securely.

It provides tools for:
- Customer Relationship Management (CRM)
- Application Development
- Automation
- Data Management
- Reports and Dashboards

Salesforce allows companies to create custom applications without needing heavy infrastructure because everything works on the cloud.

---

# 2. Explain the Following

## App

An App in Salesforce is a collection of tools, tabs, objects, and features grouped together for a specific business purpose.

Examples:
- Sales App
- Service App
- Marketing App

Apps help users access related functionalities from one place.

### Example
A Sales App may contain:
- Accounts
- Contacts
- Opportunities
- Reports

---

## Object

An Object in Salesforce is similar to a database table that stores information.

Objects contain:
- Records (rows)
- Fields (columns)

### Types of Objects
1. Standard Objects
   - Account
   - Contact
   - Opportunity

2. Custom Objects
   - Objects created by users based on business needs

### Example
A Student object can store:
- Student Name
- Roll Number
- Course

---

## Tab

A Tab is used to access objects, records, reports, dashboards, or web pages in Salesforce.

Tabs make navigation easier for users.

### Example
- Accounts Tab
- Contacts Tab
- Reports Tab

When a user clicks a tab, they can view and manage related records.

---

# 3. Difference Between Configuration and Coding
# Configuration

Configuration in Salesforce means customizing the platform using built-in tools without writing code. It is a click-based approach used to create objects, fields, validation rules, workflows, reports, dashboards, and flows. Configuration is easy to learn, faster to implement, and suitable for simple to medium business requirements. It helps administrators customize Salesforce efficiently with minimal technical knowledge.

---

# Coding

Coding in Salesforce means developing custom functionality using programming languages such as Apex, Visualforce, and Lightning Web Components (LWC). Coding is used when business requirements are complex and cannot be achieved using configuration alone. It provides more flexibility, advanced automation, and custom logic, but it requires programming skills and more development effort.

### Example

#### Configuration
- Creating fields
- Validation rules
- Workflows

#### Coding
- Writing Apex classes
- Custom integrations
- Complex automation

---

# College Management System Design

## App Name

**College Management System**

The College Management System is designed to help colleges manage student information, admissions, courses, faculty details, and daily academic activities in an organized way using Salesforce.

---

# Objects Inside the App

## Standard Objects

### Account
Used to store information about departments connected with the college.

### Contact
Used to store details of:
- Students
- Parents
- Faculty members

Information may include:
- Name
- Phone Number
- Email
- Address

---

## Custom Objects

### Student
Stores complete student information such as:
- Student ID
- Course
- Year/Semester
- Attendance
- Academic Status

### Course
Stores course details:
- Course Name
- Duration
- Subjects
- Fees

### Admission
Used to manage admission records:
- Application Number
- Admission Date
- Admission Status

### Faculty
Stores faculty information:
- Faculty Name
- Department
- Subject
- Experience

### Fees
Used to track fee payments:
- Fee Amount
- Due Date
- Payment Status

### Attendance
Stores attendance details of students.

---

# How Users Will Interact With the App

## Students
- View course details
- Check attendance
- View fee status
- Track admission information

## Faculty
- Update attendance
- Manage student records
- View course information

## Administration Staff
- Manage admissions
- Maintain student records
- Track fee payments
- Generate reports

## College Admin
- Monitor all activities
- Manage users and permissions
- Generate dashboards and reports

---

# System Workflow

1. Student applies for admission.
2. Administration verifies student details.
3. Admission is approved.
4. Student is assigned to a course.
5. Faculty updates attendance and academic details.
6. Fee payments and student records are maintained regularly.

---

![](https://github.com/24pa1a05f2-design/salesforce-training/blob/main/week%201/day2-platform-basics/Agentforce%20360%20Platform%20Basics.png?raw=true)

