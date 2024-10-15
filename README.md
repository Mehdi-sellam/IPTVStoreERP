# Enterprise Resource Planning (ERP) System for IPTV Online Store

This project is a web applicatin ERP system, developed for managing stuff, customers and stock within an IPTV online store.

## Technologies Used:
- **C#**
- **ASP.NET**
- **WebForms**
- **Event Driven Model**
- **Microsoft SQL Server** (Database is protected, further information will be provided in the future)
- **Microsoft Visual Studio 2022** (Development environment)

---

## Individual Component: Stock Management System

### Contents:
1. [Documentation](#1-documentation)
   - [Class Diagram](#11-class-diagram)
   - [Stock Use Case Diagram](#12-stock-use-case-diagram)
   - [Individual Use Case Descriptions](#13-individual-use-case-descriptions)
2. [Ethics Case Study](#2-ethics-case-study)
   - [Ethics Checklist](#21-ethics-checklist)
3. [References](#3-references)
4. [Installation](#4-Installation)
5. [Usage](#5-Usage)

---

## 1. Documentation

### 1.1 Class Diagram

![Class Diagram](https://github.com/user-attachments/assets/3402279e-86a1-4c28-98af-d2f553c2182b)

[Diagram-Preview](<https://github.com/user-attachments/assets/3402279e-86a1-4c28-98af-d2f553c2182b>)

---

### 1.2 Stock Use Case Diagram

![Use Case Diagram](https://github.com/user-attachments/assets/5ddba117-8479-4ebd-be49-7f3e799dda2a)

[Diagram-Preview](<https://github.com/user-attachments/assets/5ddba117-8479-4ebd-be49-7f3e799dda2a>)

---

### 1.3 Individual Use Case Descriptions

#### 1. Login to the system

| **Field**             | **Description**                                                                 |
|-----------------------|---------------------------------------------------------------------------------|
| **Use Case Name**      | Login to the system                                                             |
| **Use Case Description** | Granting access to the system through authentication                            |
| **Use Case Author(s)** | Dev-3                                                                           |
| **Actor(s)**           | Stock Manager                                                                   |
| **Locations**          | System user interface                                                           |
| **Primary Pathway**    | Stock manager enters the system, enters username and password, submits login form, system validates credentials and grants access. |
| **Alternate Pathways** | System suggests corrections for invalid inputs.                                  |
| **Exception Pathways** | System error during submission.                                                  |

---

#### 2. Add Stock

| **Field**             | **Description**                                                                 |
|-----------------------|---------------------------------------------------------------------------------|
| **Use Case Name**      | Add Stock                                                                       |
| **Use Case Description** | Process of adding new stock items to the system                                 |
| **Use Case Author(s)** | Dev-3                                                                           |
| **Actor(s)**           | Stock Manager                                                                   |
| **Locations**          | System user interface                                                           |
| **Primary Pathway**    | Stock manager logs in, navigates to the stock management page, enters stock details, clicks on OK, system validates and adds the stock. |
| **Alternate Pathways** | System suggests corrections for invalid inputs.                                  |
| **Exception Pathways** | System error during submission.                                                  |

---

#### 3. Edit Stock

| **Field**             | **Description**                                                                 |
|-----------------------|---------------------------------------------------------------------------------|
| **Use Case Name**      | Edit Stock                                                                      |
| **Use Case Description** | Updating details of existing stock items after searching for it.                |
| **Use Case Author(s)** | Dev-3                                                                           |
| **Actor(s)**           | Stock Manager                                                                   |
| **Locations**          | System user interface                                                           |
| **Primary Pathway**    | Stock manager logs in, navigates to the stock management page, finds specific stock, updates the details, clicks on the Edit button, system validates and updates stock. |
| **Alternate Pathways** | System suggests corrections for invalid inputs.                                  |
| **Exception Pathways** | Selected stock item not found.                                                   |

---

#### 4. Delete Stock

| **Field**             | **Description**                                                                 |
|-----------------------|---------------------------------------------------------------------------------|
| **Use Case Name**      | Delete Stock                                                                    |
| **Use Case Description** | Removing stock items from the system.                                           |
| **Use Case Author(s)** | Dev-3                                                                           |
| **Actor(s)**           | Stock Manager                                                                   |
| **Locations**          | System user interface                                                           |
| **Primary Pathway**    | Stock manager logs in, navigates to the stock management page, finds the specific stock, clicks on Delete, system removes stock item. |
| **Alternate Pathways** | Stock Manager cancels deletion.                                                  |
| **Exception Pathways** | Network failure during deletion.                                                 |

---

#### 5. Validate Stock

| **Field**             | **Description**                                                                 |
|-----------------------|---------------------------------------------------------------------------------|
| **Use Case Name**      | Validate Stock                                                                  |
| **Use Case Description** | Ensuring stock details entered meet certain criteria before adding or updating.  |
| **Use Case Author(s)** | Dev-3                                                                           |
| **Actor(s)**           | Stock Manager                                                                   |
| **Locations**          | System “internal”                                                               |
| **Primary Pathway**    | Stock manager enters stock details to add or update, system checks validation rules, system confirms or rejects validity. |
| **Alternate Pathways** | System suggests corrections for invalid inputs through output messages.          |
| **Exception Pathways** | System error during validation.                                                  |

---

#### 6. Find Stock

| **Field**             | **Description**                                                                 |
|-----------------------|---------------------------------------------------------------------------------|
| **Use Case Name**      | Find Stock                                                                      |
| **Use Case Description** | Searching for specific stock items based on Stock ID.                           |
| **Use Case Author(s)** | Dev-3                                                                           |
| **Actor(s)**           | Stock Manager                                                                   |
| **Locations**          | System user interface                                                           |
| **Primary Pathway**    | Stock manager logs in, navigates to the stock management page, enters Stock ID, clicks on the Find button, system displays stock details. |
| **Alternate Pathways** | System cannot find the wanted stock.                                             |
| **Exception Pathways** | No stock items match search criteria.                                            |

---

#### 7. List Stock

| **Field**             | **Description**                                                                 |
|-----------------------|---------------------------------------------------------------------------------|
| **Use Case Name**      | List Stock                                                                      |
| **Use Case Description** | Displaying a list of all stock items as a list from the database.               |
| **Use Case Author(s)** | Dev-3                                                                           |
| **Actor(s)**           | Stock Manager                                                                   |
| **Locations**          | System user interface                                                           |
| **Primary Pathway**    | Stock manager logs in, navigates to the stock management page, system displays all stock items. |
| **Alternate Pathways** | Stock Manager cannot find the wanted item.                                       |
| **Exception Pathways** | System error during retrieval from the database.                                 |

---

## 2. Ethics Case Study

---

### 2.1 Ethics Checklist

#### Ethical Software Development Principles

| **Key Principle** | **Rationale** | **How has it been addressed or could be addressed** |
|-------------------|---------------|----------------------------------------------------|
| **Transparency**  | Transparency is essential in the development of ethical software. Users should understand how their data is collected, processed, and stored. | Offer clear and accessible documentation regarding your software’s capabilities, limitations, and potential risks. Ensure users understand how their data is collected, processed, and stored. This openness creates trust between developers and users, allowing them to make informed decisions about their data and engagement with the platform. |
| **Privacy**       | Privacy is a fundamental right software must respect. Only collect the data required for your application’s intended purpose following the data minimization principles and acquire informed consent from users. | Collect only the data required for the intended purpose, follow data minimization principles, and ensure informed consent from users. |
| **Security**      | In ethical software development, security is paramount. Software should be planned and produced with security as a high concern. | Plan and produce software throughout the development lifecycle with security as a priority. Follow best practices to identify, avoid, and mitigate vulnerabilities. |
| **Fairness**      | Fairness ensures that software does not discriminate against any group or individual. | Ensure algorithms and decision-making processes are free of bias and do not perpetuate social and economic imbalances. Use approaches to discover and reduce biases in algorithms and data. |
| **Accountability**| The effects of software on people and society are the responsibility of its developers. | Be accountable for any unwanted outcomes, be open and honest about growth procedures, establish clear methods for reporting ethical concerns, and address issues as soon as possible. |

Source: [OpenReplay Blog on Ethical Considerations in Software Development](https://blog.openreplay.com/ethical-considerations-in-software-development/)

---

## 3. References 

- **IEEE, 2020**. *Ethically Aligned Design: A Vision for Prioritizing Human Well-being with Autonomous and Intelligent Systems, First Edition*. IEEE Standards Association. Available at: https://ethicsinaction.ieee.org/ [Accessed 30 May 2024].
- **European Union, 2018**. *General Data Protection Regulation (GDPR)*. Official Journal of the European Union. Available at: https://eur-lex.europa.eu/eli/reg/2016/679/oj [Accessed 30 May 2024].
- **ACM, 2018**. *ACM Code of Ethics and Professional Conduct*. Association for Computing Machinery. Available at: https://www.acm.org/code-of-ethics [Accessed 30 May 2024].



---
---

#### Auth: Dev-3 Mehdi Sellam   05.05.24

---
---



## 4. Installation

To install and run the ERP system locally, follow these steps:

1. **Clone the repository**:
    ```bash
    git clone https://github.com/your-username/erp-iptv-online-store.git
    ```
   
2. **Open in Visual Studio**:
   - Launch Visual Studio and open the solution file (`.sln`).

3. **Set up the Database**:
   - naviggate to Sql Server Object Explorer from the View tab from the toolbar on the right top of the screen.
   - click on add SQL Server.
   - Enter the following credentials:
   - - - Server Name: v00egd00002l.lec-admin.dmu.ac.uk
   - - - Authentification: SQL Server Authentification
   - - - User Name: ******
   - - - Password: ******

4. **Run the Application**:
   - Build and run the solution using Visual Studio.

---

## 5. Usage

Once the system is up and running, choose one of the system services stuff, stock or customers management, then log in using the default credentials (admin credentials could be found in the users table). Once you are loged in will be able to perform operations like adding, editing, deleting, and searching.

#### [Back to Contents](#Contents)
