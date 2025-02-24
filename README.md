Automatic Timetable Generator

Introduction
Managing class schedules can be a headache, especially when trying to avoid conflicts and ensure fairness. The Automatic Timetable Generator is here to solve that! This web-based tool automates the scheduling of classes, ensuring that everything runs smoothly with minimal manual effort. It uses smart algorithms to generate timetables efficiently.

What This Tool Offers
•	Easy Authentication – Secure JWT-based login/signup
•	Role-Based Access – Different permissions for Admins, Teachers, and Students
•	Smart Scheduling – Uses a Greedy Algorithm or an AI-based approach to create optimized timetables
•	Conflict-Free Timetable – Prevents class overlaps and ensures fair distribution
•	User-Friendly Interface – Simple web UI for managing schedules
•	Export Options – Download the timetable as PDF or Excel

Tech Stack
Backend:
•	Flask (Python) – Handles the logic and API requests
•	PostgreSQL – Stores all timetable data
•	SQLAlchemy – Makes database interactions smooth
•	JWT (JSON Web Token) – Keeps authentication secure

Frontend:
•	HTML, CSS, JavaScript – Simple yet effective UI
•	Fetch API – Handles smooth data updates

Other Tools:
•	Flask-Migrate – Manages database changes
•	Git & GitHub – Version control
•	Virtual Environment (venv) – Keeps dependencies organized

How to Set Up
Prerequisites:
•	Install Python (3.x)
•	Set up PostgreSQL
•	Install Git

Steps:
1.	Clone the Repository 

2.	git clone https://github.com/yourusername/automatic-timetable-generator.git

3.	cd automatic-timetable-generator/backend

4.	Set Up a Virtual Environment 

5.	python -m venv venv

6.	venv\Scripts\activate 
 
7.	Install Required Packages
 
8.	pip install -r requirements.txt

9.	Set Up Database Connection Edit your .env file with your database credentials: 

10.	DATABASE_URL=postgresql://username:password@localhost/timetable_db

11.	SECRET_KEY=your_secret_key

12.	Run the Application 

13.	flask run

API Endpoints Overview
Authentication
Endpoint       Method	   What It Does
/register	      POST	   Create a new user account
/login	        POST	   Generate an authentication token
/logout	        GET	     Log out the user

Timetable Management
Endpoint	            Method	    What It Does
/generate_timetable	   POST	      Creates a new timetable automatically
/get_timetable	       GET	      Fetches the current timetable
/update_timetable      PUT	      Allows modifications to the timetable
/delete_timetable   	 DELETE	    Removes a timetable

What’s Next?
•	AI-powered scheduling for even smarter optimization
•	Drag-and-drop timetable editing
•	Mobile-friendly interface
•	Email alerts for schedule changes

Conclusion
The Automatic Timetable Generator streamlines scheduling, reduces conflicts, and optimizes resource allocation. With a scalable design, it ensures efficiency for educational institutions.

