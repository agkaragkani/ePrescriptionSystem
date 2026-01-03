# Electronic Prescription Management System

A Java-based console application developed for the **Structured Programming (PLH 102)** course at the **Technical University of Crete**. This system simulates a digital platform for managing doctors, patients, medicines, and medical prescriptions.

## 📋 Overview

The goal of this project was to design and implement an object-oriented system that handles the lifecycle of medical prescriptions without using external databases. [cite_start]The system operates entirely in **main memory**, utilizing object associations to link patients, doctors, and medicines[cite: 70].

* [cite_start]**Course:** PLH 102 - Structured Programming [cite: 3]
* [cite_start]**Institution:** Technical University of Crete [cite: 1]
* [cite_start]**Semester:** Spring 2020 [cite: 4]

## ✨ Features

The application provides a menu-driven interface with the following functionalities:

### 1. Data Management (Registration)
* [cite_start]**Register Patients:** Stores Name and AMKA (Social Security Number)[cite: 26, 27].
* [cite_start]**Register Medicines:** Stores Name, Unique Code, and Price [cite: 30-32].
* [cite_start]**Register Doctors:** Stores Name, Specialty, and License ID [cite: 35-37].
* [cite_start]**Pre-loaded Data:** The system initializes with sample data to facilitate testing[cite: 72].

### 2. Prescription Creation
* [cite_start]**Link Entities:** Associates a specific Patient and Doctor to a new prescription[cite: 53, 55].
* [cite_start]**Medicine Selection:** Adds up to 4 medicines per prescription[cite: 44].
* [cite_start]**Validations:** Checks if the Patient, Doctor, and Medicines exist in the system before creation, returning error messages if they do not[cite: 54, 56, 58].
* [cite_start]**Automation:** Automatically calculates the total cost and assigns a unique system ID[cite: 60, 61].

### 3. Search & Reporting
* [cite_start]**Search by Patient:** Find prescriptions for a specific AMKA[cite: 63].
* [cite_start]**Search by Date:** Find prescriptions executable within a specific date range[cite: 64].
* [cite_start]**Search by Doctor:** List prescriptions written by a specific doctor[cite: 66].
* [cite_start]**Search by Medicine:** Find prescriptions containing a specific drug[cite: 67].
* [cite_start]**Print Catalogs:** Display lists of all Patients, Doctors, Medicines, or Prescriptions[cite: 68].

### 4. Deletion
* [cite_start]**Cascading Delete:** Allows deletion of a Patient by AMKA, which automatically deletes all associated prescriptions from the system[cite: 69].

## 🏗 System Architecture

The project follows a modular design with specific constraints:

* **Capacity Constraints:**
    * [cite_start]Max 100 Patients [cite: 25]
    * [cite_start]Max 100 Doctors [cite: 34]
    * [cite_start]Max 50 Medicines [cite: 28]
    * [cite_start]Max 400 Prescriptions [cite: 39]
* [cite_start]**Storage:** Non-persistent (RAM only)[cite: 70].
* [cite_start]**Input Handling:** Validates user inputs and handles navigation between the main menu and sub-functions [cite: 74-76].

## 🛠️ Built With

* **Language:** Java
* [cite_start]**IDE:** Eclipse [cite: 99]
* [cite_start]**Libraries:** `java.util.Date` for date management[cite: 104].

## 🚀 How to Run

1.  Clone this repository.
2.  Import the project into **Eclipse** as a Java Project.
3.  Locate the `Main` class.
4.  Run as **Java Application**.
5.  Follow the console prompts to navigate the menu.

---
*This project is an educational assignment created for the PLH 102 course.*