# AUTOMATIC-TIMETABLE-GENERATOR
Automatic Timetable Generator

1. Project Overview
The Automatic Timetable Generator is a web-based application designed to automate the scheduling process for educational institutions. It optimizes timetable creation by considering various constraints such as teacher availability, subject allotment, and classroom occupancy.

2. Features
•	User registration and login
•	User authentication with JWT
•	Role-based access (Admin, Faculty, Student)
•	Automated timetable generation using the Greedy Algorithm
•	Conflict resolution for overlapping schedules
•	Database-driven dynamic data handling
•	Interactive UI for viewing, updating, and managing timetables
•	Export timetable as PDF or Excel

3. Tech Stack
  •	Backend: Flask (Python)
  •	Database: PostgreSQL
  •	Frontend: HTML, CSS, JavaScript
  •	Authentication: JWT
  •	Algorithm: Greedy Algorithm 

4. System Architecture
  1.Frontend: The user interface allows admins to configure constraints, faculty to view schedules, and students to access timetables.
  2.Backend: Handles authentication, processes scheduling logic, and communicates with the database.
  3.Database: Stores user data, timetable information, faculty availability, and constraints.
  4.Algorithm Engine: Implements the Greedy Algorithm to optimize and generate an efficient timetable.

5. Installation & Setup

Prerequisites
  •	Python 3.x
  •	PostgreSQL
  •	HTML, CSS and JavaScript 
  •	Virtual Environment 
  •	Flask

Steps
  1. Clone the Repository
     git clone <repository-url>
     cd automatic-timetable-generator

  2. Set Up a Virtual Environment
     python -m
     venv\Scripts\activate

  3. Install Dependencies
      pip install -r requirements.txt

  4. Configure the Database
     •Create a PostgreSQL database
     •Update config.py with database credentials

  5. Start the Flask Server
      flask run


  6. API Endpoints
      Method	Endpoint	Description
     POST	/register	User registration
     POST	/login	User authentication
     GET	/timetable	Retrieve generated timetable
     POST	/generate	Trigger timetable generation


  7. Timetable Generation Algorithm 
     The scheduling algorithm follows these steps:
        1.	Gather Input: Fetch faculty, subjects, and constraints from the database.
        2.	Sort by Priority: Sort classes based on constraints (e.g., faculty preferences, subject difficulty).
        3.	Slot Allocation: Assign time slots while resolving conflicts.
        4.	Validate Constraints: Check for clashes and reallocate if necessary.
        5.	Store & Display: Save the generated timetable and provide API access.

8. Future Enhancements
 •Implement AI-based optimization (Genetic Algorithm)
 •Add drag-and-drop timetable editor
 •Integrate notifications for schedule updates

9. Conclusion
The Automatic Timetable Generator streamlines scheduling, reduces conflicts, and optimizes resource allocation. With a scalable design, it ensures efficiency for educational institutions.

