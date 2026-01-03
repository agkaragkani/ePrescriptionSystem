# Electronic Prescription Management System

A Java-based console application developed for the **Structured Programming (PLH 102)** course at the **Technical University of Crete**. This system simulates a digital platform for managing doctors, patients, medicines, and medical prescriptions.

## 📋 Overview

The goal of this project was to design and implement an object-oriented system that handles the lifecycle of medical prescriptions without using external databases.The system operates entirely in **main memory**, utilizing object associations to link patients, doctors, and medicines.

**Course:** PLH 102 - Structured Programming 
**Institution:** Technical University of Crete 
**Semester:** Spring 2020 
## ✨ Features

The application provides a menu-driven interface with the following functionalities:

### 1. Data Management (Registration)
**Register Patients:** Stores Name and AMKA (Social Security Number).
**Register Medicines:** Stores Name, Unique Code, and Price.
**Register Doctors:** Stores Name, Specialty, and License ID.
**Pre-loaded Data:** The system initializes with sample data to facilitate testing.

### 2. Prescription Creation
**Link Entities:** Associates a specific Patient and Doctor to a new prescription.
**Medicine Selection:** Adds up to 4 medicines per prescription.
**Validations:** Checks if the Patient, Doctor, and Medicines exist in the system before creation, returning error messages if they do not[cite: 54, 56, 58].
**Automation:** Automatically calculates the total cost and assigns a unique system ID.

### 3. Search & Reporting
**Search by Patient:** Find prescriptions for a specific AMKA.
**Search by Date:** Find prescriptions executable within a specific date range.
**Search by Doctor:** List prescriptions written by a specific doctor.
**Search by Medicine:** Find prescriptions containing a specific drug.
**Print Catalogs:** Display lists of all Patients, Doctors, Medicines, or Prescriptions.

### 4. Deletion
**Cascading Delete:** Allows deletion of a Patient by AMKA, which automatically deletes all associated prescriptions from the system.

## 🏗 System Architecture

The project follows a modular design with specific constraints:

**Capacity Constraints:**
    *Max 100 Patients
    *Max 100 Doctors 
    *Max 50 Medicines
    *Max 400 Prescriptions 
**Storage:** Non-persistent (RAM only).
**Input Handling:** Validates user inputs and handles navigation between the main menu and sub-functions.

## 🛠️ Built With

**Language:** Java
**IDE:** Eclipse 
**Libraries:** `java.util.Date` for date management.

## 🚀 How to Run

1.  Clone this repository.
2.  Import the project into **Eclipse** as a Java Project.
3.  Locate the `Main` class.
4.  Run as **Java Application**.
5.  Follow the console prompts to navigate the menu.

---
*This project is an educational assignment created for the PLH 102 course.*
