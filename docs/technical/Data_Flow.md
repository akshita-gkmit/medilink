# Data Flow diagram
The **Data Flow Diagram (DFD)** of MediLink illustrates how information travels between different entities **Patients**, **Doctors**, **Admins**, and the core system modules.  

MediLink’s architecture is divided into interconnected functional components:  

- **Authentication Module (FUC-01 & FUC-07):** Handles user registration, login, and secure token generation using JWT.  
- **Doctor Management (FUC-02):** Allows admins to add, edit, or remove doctor profiles and update their details in the database.  
- **Slot Management (FUC-03):** Enables doctors to define their consultation timings, availability, and updates these slots in real-time.  
- **Appointment Management (FUC-04, FUC-05, FUC-06):** Manages the patient’s booking, doctor’s approval/rejection, and database synchronization.  

Each user interacts with the **Authentication Module** first, which validates their identity and grants access to role-specific features. The modules communicate with the central **database** for storing and retrieving data, ensuring synchronization between user actions and system records.  

This data flow ensures smooth communication, role-based access control, and consistent updates across the MediLink system providing a secure and efficient healthcare management experience.

![Data Flow Diagram](../images/dfd.png)