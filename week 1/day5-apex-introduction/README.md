# Day 5 - Apex Introduction

## 1. What is Apex?

Apex is a programming language developed by Salesforce.  
It is mainly used to add custom business logic inside Salesforce applications.

With Apex, developers can:
- Automate processes
- Create custom validations
- Connect Salesforce with external systems
- Write triggers and classes
- Build advanced functionality that cannot be done only with configuration tools

In simple words, Apex helps developers customize Salesforce according to business needs.

---

# 2. Difference

## Flow vs Apex

| Flow | Apex |
|------|------|
| Flow is a no-code or low-code automation tool | Apex is a coding language |
| Easy to create using drag-and-drop | Requires programming knowledge |
| Best for simple automation | Best for complex logic |
| Faster for admins to build | More flexible for developers |
| Limited for advanced operations | Can handle advanced customizations |

### Example
- Sending an email automatically → Flow  
- Complex fee calculation with multiple conditions → Apex

---

## Configuration vs Coding

| Configuration | Coding |
|--------------|---------|
| Uses clicks instead of code | Uses programming languages |
| Easier to maintain | Requires development skills |
| Good for standard features | Good for advanced requirements |
| Faster implementation | More customizable |
| Used by admins | Used by developers |

### Example
- Creating fields and validation rules → Configuration  
- Creating custom admission logic → Coding

---

# 3. Real Examples Where Apex Is Needed

## 1. Automatic Scholarship Eligibility
When a student applies for admission, Apex can automatically check marks, income, and category details to decide scholarship eligibility.

## 2. Attendance Warning System
Apex can automatically send warning emails to students whose attendance goes below a certain percentage.

## 3. Fee Due Reminder
Apex can generate reminders and notifications for students who did not pay fees before the deadline.

---

# 4. Integrated System Design

## College Management System Using Salesforce

### CRM
The College Management System uses Salesforce CRM to manage student data, admissions, courses, faculty information, and communication.

---

## Objects

### Standard Objects
- Account → Schools or Colleges
- Contact → Students or Parents

### Custom Objects
- Student
- Course
- Admission
- Attendance
- Fees
- Faculty

---

## Relationships

- One student can enroll in many courses
- One faculty member can teach multiple courses
- One student can have multiple fee records
- Admission records are linked with students

---

## Validation

Validation rules help maintain correct data.

### Examples
- Phone number must contain 10 digits
- Student ID should be unique
- Fee amount cannot be negative
- Admission date cannot be in the past

---

## Flow

Flows can automate simple processes.

### Examples
- Send welcome email after admission
- Create fee record automatically
- Notify faculty when a student enrolls in a course

---

## Apex

Apex is used when the business logic becomes complex.

### Examples
- Calculate scholarship eligibility
- Generate attendance alerts
- Create semester performance reports
- Integrate payment systems with Salesforce

---

# 5. Pseudocode Examples

## Scholarship Eligibility

```text
START

IF student marks > 85
AND family income < limit
THEN
    Scholarship = Approved
ELSE
    Scholarship = Not Approved

 END
```

```text
START

IF attendance percentage < 75
THEN
    Send warning email to student

 END
```

# 6. Reflection

Enterprise systems become more complex as organizations grow.
At the beginning, configuration tools are enough for simple tasks. But when businesses require advanced automation, integrations, calculations, and custom processes, programming becomes necessary.
Apex helps organizations build scalable and flexible solutions that match real business requirements. It allows developers to create smarter systems that improve efficiency, reduce manual work, and provide better user experiences.