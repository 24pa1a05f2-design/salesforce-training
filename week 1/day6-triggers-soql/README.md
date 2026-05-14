

## 1. What is SOQL?

SOQL (Salesforce Object Query Language) is used to retrieve records from Salesforce objects.  
It is similar to SQL, but it is specially designed for Salesforce data and relationships.


---

## 2. What is an Apex Trigger?

An Apex Trigger is a piece of Apex code that automatically executes when data changes in Salesforce.  
Triggers are commonly used for automation, validation, and updating related records.

### Example:
- Automatically send notifications when attendance becomes low.
- Create fee reminders for students with pending payments.

---

## 3. Difference

### Flow vs Trigger

| Flow | Trigger |
|------|---------|
| Point-and-click automation | Code-based automation |
| Easy for admins | Used by developers |
| Best for simple automation | Best for complex logic |
| No coding required | Requires Apex programming |

### Before vs After Trigger

| Before Trigger | After Trigger |
|---------------|---------------|
| Runs before saving record | Runs after saving record |
| Used to update field values | Used for related actions |
| Faster because data is not committed | Used when Record ID is needed |

---

## 4. Trigger Use Cases – College Management System

1. Automatically send an email to students when attendance drops below 75%.  
2. Create a fee reminder task when fee due date is reached.  
3. Update student status after course completion.  
4. Prevent duplicate student registrations using validation logic.  
5. Automatically assign faculty when a new course is created.  

---

## 5. Query Examples

### Find all students in Course A
```sql
SELECT Name FROM Student__c WHERE Course__c = 'Course A'
```

### Find all courses handled by Faculty X
```sql
SELECT Name FROM Course__c WHERE Faculty__c = 'Faculty X'
```

### Find students with attendance below 75%
```sql
SELECT Name, Attendance__c FROM Student__c WHERE Attendance__c < 75
```

### Find faculty teaching more than 3 courses
```sql
SELECT Name FROM Faculty__c WHERE Total_Courses__c > 3
```

### Find students who registered this month
```sql
SELECT Name FROM Student__c WHERE CreatedDate = THIS_MONTH
```

---

## 6. Reflection

Enterprise systems react automatically to data changes because organizations handle large amounts of information daily.  
Manual processing takes more time and may lead to errors, so automation helps systems work faster and more accurately.  
Using Triggers and event-driven behavior ensures smooth operations and better user experience in applications like college management systems.