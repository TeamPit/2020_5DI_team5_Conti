Architecture Document

**EG Service**

1.0 Introduction

The EG Service document is designed to illustrate the high-level architecture systems managed to design and implement our application. The document contains a general view of the system hierarchy, logical views of the system components and a view of the system communication process.

2.0 High Level Hierarchy

**2.1 Hierarchy Diagram**

![](RackMultipart20200419-4-g5afjq_html_ef1ff57236863d5b.png)

**2.2 Hierarchy Description**

The architecture system for the EG Service application is a level n architecture. This architecture system is set up to allow the correct hiding of information, modular components and dependencies of the individual system. The database level is the last level in the hierarchy.

3.0 Components Classification

**3.1 Presentation Layer**

**Purpose:** to create the user that will be easily usable by the user

**Specific nature** : the presentation level will have the task of presenting in a dynamic and user-friendly way

**3.2 Controller Layer**

**Purpose:** Responds to user events

**Specific Nature:** the level controller in our program will be commissioned by the main server and the database

**3.3 Business Layer**

**Purpose:** this level is responsible for business logic.

**Specific Nature:** this level will be used to bring the customer to purchase the largest number of items.

**3.4 Record Layer**

**Purpose:** this level has the task of containing the classes which are strictly made up of data.

**Specific Nature:** the level will be used to store user data, with purchase credentials etc.

**3.5 Database Layer**

**Purpose:** This layer is in charge of storing data

**Specific Nature:** this level represents the stable part of the application and will be managed with the use of XML files.
