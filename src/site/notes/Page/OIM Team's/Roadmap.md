---
{"dg-publish":true,"permalink":"/page/oim-team-s/roadmap/","noteIcon":""}
---

 
## **Phase 1: Computing Fundamentals**

Before learning OIM, it’s essential to have a good understanding of basic computing concepts. These are foundational knowledge that will help you understand how systems like OIM work at a technical level.

### **1.1 Basic Computer Concepts**
1. **CPU (Central Processing Unit)**:
   - The "brain" of the computer. It processes instructions and performs tasks.
   - Types of CPUs: Single-core, multi-core.
   - Clock Speed: Measured in GHz, indicates how fast the CPU can process instructions.

2. **RAM (Random Access Memory)**:
   - Temporary memory used by the computer to store data that is being actively used.
   - Important for running applications and multitasking. More RAM allows more programs to run simultaneously.

3. **ROM (Read-Only Memory)**:
   - Permanent memory used to store firmware, or essential code that does not change, like the BIOS of a computer.

4. **Storage Devices**:
   - **Hard Disk Drive (HDD)**: Mechanical storage device with larger capacity but slower speed.
   - **Solid-State Drive (SSD)**: Faster than HDD with no moving parts, used for rapid data retrieval.

5. **File Types**:
   - **.exe**: Executable files for launching programs.
   - **.txt**: Plain text files.
   - **.csv**: Comma-separated values, used for structured data like spreadsheets.
   - **.jar**: Java Archive files, used for Java programs.
   - **.xml/.json**: Data representation files, commonly used in APIs and configuration.

6. **Networking Basics**:
   - **IP Address**: Unique identifier for devices on a network.
   - **Protocols**: HTTP, HTTPS, FTP, SMTP, etc.
   - **Firewall**: A network security device that monitors incoming and outgoing network traffic.

---

## **Phase 2: Java Programming (Basic to Advanced)**

OIM is built on Java, so understanding Java concepts is crucial for developing and customizing OIM. Below is a structured path to learn Java, starting from basics and advancing to the level required for OIM development.

### **2.1 Java Fundamentals**
1. **Setting up Java Environment**:
   - Install JDK (Java Development Kit).
   - Set up your Integrated Development Environment (IDE) such as IntelliJ IDEA or Eclipse.

2. **Basic Java Concepts**:
   - **Variables and Data Types**: int, float, char, boolean, String.
   - **Operators**: Arithmetic, comparison, logical operators.
   - **Control Flow**: if-else, switch-case, loops (for, while, do-while).

3. **Object-Oriented Programming (OOP) Concepts**:
   - **Classes and Objects**: Blueprint of an object, creating instances.
   - **Methods**: Defining and calling methods (functions in Java).
   - **Encapsulation**: Data hiding using private variables and public getters/setters.
   - **Inheritance**: Allowing a class to inherit properties from another class.
   - **Polymorphism**: Method overloading and overriding.
   - **Abstraction**: Abstract classes and interfaces to define the structure without implementation.
   - **Constructors**: Special methods used to initialize objects.

4. **Collections Framework**:
   - **ArrayList, LinkedList, HashMap, HashSet**: Understand the basic data structures available in Java.
   - **Iterating through collections** using loops and iterators.

5. **Exception Handling**:
   - **Try-Catch-Finally**: Handling errors in your code.
   - **Checked vs Unchecked Exceptions**: Understand the difference and when to use each.
   - **Custom Exceptions**: Creating your own exceptions.

6. **Java I/O**:
   - **Reading/Writing Files**: InputStream, OutputStream, Reader, Writer.
   - **Working with XML and JSON**: Parsing and generating XML/JSON.

### **2.2 Advanced Java Concepts**
1. **Multithreading**:
   - **Thread class and Runnable interface**: Understand how Java handles parallel tasks.
   - **Synchronization**: Managing shared resources between threads.
   - **Executor Framework**: Using thread pools for task management.

2. **Java 8 Features**:
   - **Lambda Expressions**: Functional programming in Java.
   - **Streams API**: Processing collections of objects.
   - **Functional Interfaces**: Predicate, Consumer, Supplier.

3. **JDBC (Java Database Connectivity)**:
   - Connecting to databases from Java.
   - Executing SQL queries, handling results.

4. **RESTful Web Services**:
   - Using **JAX-RS** to develop and consume REST APIs.
   - Handling HTTP requests/responses.

---

## **Phase 3: OIM Fundamentals**

Once you have a good grasp of Java, you can move on to learning Oracle Identity Manager basics.

### **3.1 What is Oracle Identity Manager (OIM)?**
- OIM is a comprehensive identity management solution from Oracle that automates the provisioning and de-provisioning of user accounts across systems and applications.
  
### **3.2 Core Concepts in OIM**
1. **Provisioning and De-provisioning**:
   - **Provisioning**: Assigning user access and accounts to resources like databases or applications.
   - **De-provisioning**: Removing access when it's no longer needed.

2. **Role-Based Access Control (RBAC)**:
   - **Roles**: Groups that define access privileges for users.
   - **Entitlements**: Specific permissions assigned to a role.

3. **User Lifecycle Management**:
   - Managing user accounts from creation, modification, and deactivation.

4. **Connectors**:
   - OIM uses connectors to communicate with external systems (e.g., Active Directory, databases).
   - **Pre-built connectors**: OIM comes with ready connectors for common systems like LDAP, Salesforce, etc.
   - **Custom connectors**: Developers can create connectors for non-standard systems.

5. **Reconciliation**:
   - Synchronizing data between OIM and external systems.
   - **Trusted Reconciliation**: Data flows from the trusted system (e.g., HR system) to OIM.
   - **Target Reconciliation**: Data flows from OIM to the target system.

### **3.3 OIM Architecture**
1. **OIM Server**: The central server that manages identity management tasks.
2. **Database**: Stores user data, configurations, and audit logs.
3. **WebLogic Server**: Application server used to run OIM.
4. **OIM Design Console**: A client application used by developers to configure and manage OIM workflows, rules, and forms.

---

## **Phase 4: OIM Development**

With Java knowledge and a good understanding of OIM concepts, you can now move on to OIM development. This phase focuses on customization, extending OIM functionalities, and developing custom connectors.

### **4.1 OIM Customization**
1. **OIM API (Java API)**:
   - **User Management**: Creating, updating, and managing user data through API.
   - **Provisioning Management**: Automating provisioning and de-provisioning tasks using API calls.
   - **Role Management**: Managing roles and entitlements using the API.

2. **Event Handlers**:
   - Java classes that listen to events (e.g., user creation, modification) and perform actions based on these events.
   - **Types of Event Handlers**: Pre-process, post-process, and conditional event handlers.
   - **Use cases**: Automatically adding entitlements when a user is created.

3. **Custom Adapters**:
   - Code that automates certain actions in OIM, such as pre-populating fields or assigning tasks.

4. **UI Customization**:
   - Customizing the OIM web interface using the Oracle Identity Self Service Console.
   - Adding custom fields, modifying forms, and changing approval workflows.

### **4.2 Developing Custom Connectors**
1. **Introduction to OIM Connectors**:
   - Custom connectors allow OIM to communicate with external systems that don’t have out-of-the-box support.

2. **Creating Custom Connectors**:
   - Develop Java-based connectors for integrating with non-standard systems.
   - Use the **Connector Framework** for building, testing, and deploying these connectors.

### **4.3 SOA (Service-Oriented Architecture) Integrations**
- Integrating OIM with Oracle SOA Suite for advanced business process automation.
- **BPEL (Business Process Execution Language)** workflows for handling complex multi-step processes in identity management.

### **4.4 Debugging and Troubleshooting in OIM**
- **Log Files**: Understanding the key log files for troubleshooting (WebLogic logs, OIM logs).
- **Debugging Tools**: Using breakpoints, stack traces, and error logs to debug OIM code.
  
### **4.5 Deployment Best Practices**
1. **Testing in Sandbox**: Deploy and test customizations in a sandbox environment before moving to production.
2. **Moving to Production**: Steps for safely deploying custom connectors, adapters, and other customizations to the live system.

---
