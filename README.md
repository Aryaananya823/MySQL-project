Hospital Management System Database:
        This project represents the SQL schema for a Hospital Management System that manages various aspects of hospital operations, including patient information, doctor schedules, appointments, medical history, and diagnoses. The database is structured to facilitate the management of patient records, doctor availability, appointment scheduling, and medical diagnosis history.

Database Schema Overview:
        The schema consists of several tables, each serving a specific function to manage the hospital's data efficiently. Below is a brief description of each table:
    
1. Schema: hospital_management:      
        The main schema that includes all the hospital-related tables.
2. Tables

    patient: Stores information about patients including email, password, name, address, and gender.
        medical_history: Stores a patient's medical history, including conditions, surgeries, and medication.
   
   doctor: Stores information about doctors, including email, name, gender, and password.
   
    appointment: Contains appointment details such as appointment ID, date, start and end times, and status.
   
    patient_visits: Tracks patient visits, concerns, symptoms, and references the appointment details.
   
      schedule: Maintains the schedules of doctors, including working hours, break times, and days.
   
    patients_history: Links patients to their medical histories.
   
    diagnose: Stores diagnosis and prescription details linked to appointments and doctors.
   
    doctor_schedules: Links doctors to their working schedules.
   
     doctor_view_history: Tracks which doctors have viewed a patient's medical history.


4. Additional Schema: online_retail_app

5.user_login: Stores user login credentials for the hospital's online retail system, with fields for user ID, password, name, sign-up date, and email.
SQL Scripts:
		The provided SQL scripts drop and create the necessary schemas and tables if they don't already exist. The CASCADE option ensures that dependent objects are also removed when dropping the schema or tables.

Key Constraints and Relationships
Foreign keys are used extensively to maintain relationships between patients, doctors, appointments, medical history, and schedules.
Unique and primary key constraints are enforced to ensure data integrity.
SERIAL data types are used for auto-incrementing primary keys where necessary.
