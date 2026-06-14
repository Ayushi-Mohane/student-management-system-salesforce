# Student Management System (Salesforce Admin Project)
## Project Overview

This project demonstrates Salesforce Administration concepts by building a Student Management System. The system helps manage students, courses, and enrollments using Salesforce customization features such as custom objects, master-detail relationships, validation rules, record types, flow automation, reports, and dashboards.

The application automates the student enrollment process and provides analytical insights through reports and dashboards for better decision-making.
## Platform Used
Salesforce Lightning Platform
CRM Customization Features

## Custom Objects
Created Custom Objects:

Student 
Course
Enrollment

Fields Created
## Student Object

| Field Name | Data Type |
|------------|------------|
| Student ID | Auto Number |
| Name | Text |
| Email | Email |
| Phone | Phone |
| Department | Picklist |
| Category | Picklist |
| Semester | Picklist |
| Scholarship Percentage | Number |
| Graduation Year | Number |
| Status | Picklist |

## Course Object

| Field Name | Data Type |
|------------|------------|
| Course Name | Text |
| Duration Months | Number |
| Fees | Currency |
| Type | Picklist |

## Enrollment Object

| Field Name | Data Type |
|------------|------------|
| Enrollment ID | Auto Number |
| Enrollment Date | Date |
| Payment Status | Picklist |
| Student | Master-Detail(Student) |
| Course | Master-Detail(Course) |


## Relationships

## Validation Rules

## Flow Automation

## Reports & Dashboard            

## Skills Demonstrated
