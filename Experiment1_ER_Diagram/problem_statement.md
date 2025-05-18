# Experiment 1: Entity-Relationship (ER) Diagram

## 🎯 Objective:
To understand and apply the concepts of ER modeling by creating an ER diagram for a real-world application.

## 📚 Purpose:
The purpose of this workshop is to gain hands-on experience in designing ER diagrams that visually represent the structure of a database including entities, relationships, attributes, and constraints.

---

## 🧪 Choose One Scenario:

### 🔹 Scenario 1: University Database
Design a database to manage students, instructors, programs, courses, and student enrollments. Include prerequisites for courses.

**User Requirements:**
- Academic programs grouped under departments.
- Students have admission number, name, DOB, contact info.
- Instructors with staff number, contact info, etc.
- Courses have number, name, credits.
- Track course enrollments by students and enrollment date.
- Add support for prerequisites (some courses require others).

---

### 🔹 Scenario 2: Hospital Database
Design a database for patient management, appointments, medical records, and billing.

**User Requirements:**
- Patient details including contact and insurance.
- Doctors and their departments, contact info, specialization.
- Appointments with reason, time, patient-doctor link.
- Medical records with treatments, diagnosis, test results.
- Billing and payment details for each appointment.

---

## 📝 Tasks:
1. Identify entities, relationships, and attributes.
2. Draw the ER diagram using any tool (draw.io, dbdiagram.io, hand-drawn and scanned).
3. Include:
   - Cardinality & participation constraints
   - Prerequisites for University OR Billing for Hospital
4. Explain:
   - Why you chose the entities and relationships.
   - How you modeled prerequisites or billing.

# ER Diagram Submission - Student Name

## Scenario Chosen:
University

## ER Diagram:
![Screenshot 2025-05-18 174008](https://github.com/user-attachments/assets/f84922ca-7d2a-409c-b50b-55144fac7317)


## Entities and Attributes:
Student: Name, Date of Birth, Admission ID, Phone Number<br>
Instructor: Staff Name, Staff Number, Phone Number, Staff E-mail<br>
Course: Course Number, Course Name, Course Credit, Course Units<br>
Enrollment: Student ID, Student Enrolled Course, Date of Enrolment<br>
...

## Relationships and Constraints:
University (One-to-Many, Total Participation from Student, Instructor, and Course)<br>
Enrollment (Many-to-Many, Total Participation from Student, Partial Participation from Course)<br>
...

## Extension (Billing):
The Billing extension adds a new entity with attributes like Billing ID, Student ID, Total Amount, Billing Date, and Payment Status. It has a one-to-many relationship with the Student entity—each student can have multiple billing records. This relationship shows total participation from Billing and partial participation from Student, allowing effective tracking of student payments.

## Design Choices:
Brief explanation of why you chose certain entities, relationships, and assumptions

## RESULT
