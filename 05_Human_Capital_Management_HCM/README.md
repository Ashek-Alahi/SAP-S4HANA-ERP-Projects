# SAP HCM (Human Capital Management) – Human Resource Management System Development

## Project Overview

This project demonstrates the implementation of core Human Resource Management (HRM) functions in SAP HCM. The objective was to configure organizational management structures, create employee qualifications, assign competencies, and perform employee hiring processes using standard SAP HCM transactions.

---

## Team Members

| Name                        | Student ID |
| --------------------------- | ---------- |
| Alahi Ashek                 | M23W0308   |
| Angage Isuru Lakshan Perera | M23W0147   |
| Thapa Anjuli                | M23W7501   |

---

## SAP Module

**SAP HCM (Human Capital Management)**

Key Areas Covered:

* Organizational Management (OM)
* Personnel Administration (PA)
* Qualifications Management
* Recruitment & Employee Hiring

---

## Project Objectives

* Configure organizational units and staffing structures.
* Create and manage employee qualifications.
* Assign qualifications to positions.
* Hire new employees using SAP HCM Personnel Administration.
* Demonstrate a simplified recruitment and onboarding workflow.

---

## SAP HCM Overview

SAP Human Capital Management (HCM) helps organizations manage:

* Personnel Administration
* Organizational Management
* Payroll Processing
* Benefits Administration
* Time Management
* Recruitment and Talent Acquisition

---

## Business Scenario

The organization required modifications to its security department structure and recruitment process.

### Requirements

* Change organizational start date to **01.10.2023**
* Create new sub-organizational units
* Create security positions
* Transfer positions between organizational units
* Create and assign qualifications
* Hire a new employee

---

## Project Activities

### 1. Organizational Management (PPOME)

#### Created Sub-Organizational Units

Under **Security Organizational Unit**:

* Plant Security
* IT Security

#### Created Positions

Under **IT Security**:

* Security Guard
* Security Manager

#### Position Transfer

Transferred positions:

* 078 Security Guard
* 078 Security Manager

To:

* 078 Plant Security

**Transaction Code:** `PPOME`

---

### 2. Qualification Management (OOQA)

#### Qualification Group Created

* 078 Soft Skills

#### Qualification Created

* 078 IT Affinity

**Transaction Code:** `OOQA`

---

### 3. Qualification Assignment (PPPM)

Assigned:

| Qualification   | Proficiency Level |
| --------------- | ----------------- |
| 078 IT Affinity | Very Good         |

**Transaction Code:** `PPPM`

---

### 4. Personnel Administration – Hiring Process (PA40)

Performed employee hiring process using:

**Transaction Code:** `PA40`

Activities:

* New Hire Action
* Employee Master Data Creation
* Personnel Assignment
* Employment Record Creation

---

## Recruitment Process in SAP HCM

1. Identify Job Requirements
2. Create Job Opening
3. Advertise Position
4. Receive Applications
5. Review Candidate Profiles
6. Conduct Interviews
7. Select Candidate
8. Hire Employee
9. Employee Onboarding

---

## Transaction Codes Used

| Transaction | Description                |
| ----------- | -------------------------- |
| PPOME       | Organization and Staffing  |
| OOQA        | Create Qualifications      |
| PPPM        | Assign Qualifications      |
| PA40        | Personnel Actions (Hiring) |

---

## Learning Outcomes

Through this project, we learned how to:

* Manage organizational structures in SAP HCM.
* Create and maintain qualifications.
* Assign competencies to employees and positions.
* Execute personnel hiring actions.
* Understand recruitment workflows within SAP ERP.

---

## Project Contribution

| Member                                 | Contribution                                               |
| -------------------------------------- | ---------------------------------------------------------- |
| Angage Isuru Lakshan Perera (M23W0147) | SAP System Configuration and Execution                     |
| Alahi Ashek (M23W0308)                 | Documentation, Presentation Preparation, Slide Development |
| Thapa Anjuli (M23W7501)                | Information Collection and Project Support                 |

---

## Technologies Used

* SAP ERP HCM
* SAP GUI
* Organizational Management
* Personnel Administration
* Qualifications Management

---

## Project Status

✅ Completed

Academic ERP Project – SAP Human Capital Management (HCM)
