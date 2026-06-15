# Student Management System (Salesforce Admin Project)
## Project Overview

This project demonstrates Salesforce Administration concepts by building a Student Management System. The system helps manage students, courses, and enrollments using Salesforce customization features such as custom objects, master-detail relationships, validation rules, record types, flow automation, reports, and dashboards.

The application automates the student enrollment process and provides analytical insights through reports and dashboards for better decision-making.
## Platform Used
* Salesforce Lightning Platform

* CRM Customization Features

## Custom Objects
Created Custom Objects:

* Student 

* Course

* Enrollment

Fields Created
## Student Object

| Field Name | Data Type |
|------------|------------|
| Student ID | Auto Number |
| Name | Text |
| Email | Email |
| Phone | Phone |
| Department | Picklist(Computer Engineering, Civil Engineering, Mechanical Engineering, Electrical Engineering, Electrical Engineering, Electronics Engineering, Information Technology)|
| Category | Picklist (Open, OBC, SC, ST, EWS) |
| Semester | Picklist  |
| Scholarship Percentage | Number |
| Graduation Year | Number |
| Status | Picklist (New, Enrolled, Active) |
| City | Text | 
| Date of Birth | Date |
|Admission Year | Number | 

## Course Object

| Field Name | Data Type |
|------------|------------|
| Course Code | Auto Number |
| Course Name | Text |
| Duration Months | Number |
| Fees | Currency |
| Type | Picklist (Core, Elective, Laboratory, Project) |

## Enrollment Object

| Field Name | Data Type |
|------------|------------|
| Enrollment ID | Auto Number |
| Enrollment Date | Date |
| Payment Status | Picklist (Pending, Partially Paid, Paid) |
| Student | Master-Detail(Student) |
| Course | Master-Detail(Course) |


## Validation Rules

### Student Object
- Email Validation – Ensures valid email format.
- Phone Number Validation – Ensures phone numbers contain exactly 10 digits.
- Admission Year Validation – Prevents future admission years.

### Course Object
- Course Fee Validation – Ensures fee is greater than zero.
- Duration Validation – Ensures duration is greater than zero.

### Enrollment Object
- Enrollment Date Validation – Prevents future enrollment dates.
## Record Types

Record Types were implemented on the Student object to support different categories of students and allow future customization of business processes, page layouts, and picklist values.

### Record Types Created

1. Undergraduate
2. Postgraduate

### Purpose

* Differentiate undergraduate and postgraduate students.
* Support future customization of admission processes.
* Allow separate page layouts and picklist values if required.
* Improve data organization and scalability.


## Flow Automation

### Enrollment Payment Automation

A Record-Triggered Flow was created on the Enrollment object to automate the enrollment process when a student's payment is completed.

#### Trigger Condition

Payment Status = Paid

#### Automation Actions

##### 1. Update Student Status

When the Payment Status is marked as **Paid**, the related Student record is automatically updated and the Student Status is changed to **Enrolled**.

##### 2. Send Enrollment Confirmation Email

When the Payment Status is marked as **Paid**, an enrollment confirmation email is automatically sent to the student.

#### Business Benefits

* Eliminates manual updates to student records.
* Ensures accurate enrollment tracking.
* Improves communication through automated email notifications.
* Reduces administrative effort and human error.


## Reports & Dashboard            

## Reports & Dashboard

### Reports

* Students Per Course
* Enrollments by Payment Status
* Students by Department
* Students by Category
* Students by Semester

### Dashboard

A Student Management Dashboard was created to visualize enrollment and student data using:

* Students Per Course
* Enrollments by Payment Status
* Students by Department
* Students by Category
* Students by Semester


## Skills Demonstrated 

* Salesforce Administration
* Data Modeling
* Custom Objects
* Master-Detail Relationships
* Record Types
* Validation Rules
* Flow Builder
* Email Automation
* Reports & Dashboards
* CRM Concepts

