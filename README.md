🐾 Pet Adoption System
A full-featured pet adoption web application built with Java Servlets, JSP, JDBC, and MySQL. It supports admin, shelter, and adopter dashboards for efficient pet management and adoption workflows.

🚀 Features
User Registration & Login (Admin, Shelter, Adopter roles)

Admin Dashboard:
User management, shelter management, pet management, adoption request tracking

Shelter Dashboard:
Manage shelter info, add/edit pets, review requests

Adopter Dashboard:
Search pets, view own requests, track adoption status

Pet Management:
Create/update/delete pets, search, filter, status (available/adopted/pending)

Adoption Request Workflow:
Request pet adoption, approve/reject requests

Responsive UI:
Modern look using custom CSS styles and gradients

📦 Tech Stack
Backend: Java Servlet API, JSP

Frontend: HTML, CSS (custom, clean and responsive)

Database: MySQL (JDBC)

Server: Apache Tomcat 9.0+

Build: IntelliJ IDEA Artifacts / WAR packaging

Version: Java 8+

🗃️ Directory Structure
text
PetAdoptionSystem/
├── src/
│   └── main/
│        ├── java/                 # Java classes (Servlets, DAO, Models)
│        └── webapp/               # JSPs, static files
│           └── WEB-INF/           # web.xml, classes, libraries
├── sql/
│    └── schema.sql                # Database schema and sample data
├── pom.xml / build.gradle         # (if using Maven/Gradle)
└── README.md


🔧 Setup & Installation

1. Clone the repo
bash
git clone https://github.com/your-username/pet-adoption-system.git
cd pet-adoption-system

2. Set up MySQL
Import sql/schema.sql in your MySQL DB.

Configure your database credentials in DAO classes.

3. Configure and Build Project
Open in IntelliJ IDEA.

Build Artifact → Create WAR (check src/main/webapp is included in output).

4. Deploy to Tomcat
Copy the generated .war file into your Tomcat webapps folder.

Start Tomcat (startup.bat).

5. Access in Browser
text
http://localhost:8080/PetAdoptionSystem/home.jsp

🖥️ Screenshots
![WhatsApp Image 2025-11-25 at 14 44 19_c723c173](https://github.com/user-attachments/assets/0abfb637-0026-4405-a50d-63d2c9d16375)

![WhatsApp Image 2025-11-25 at 14 44 19_612ee921](https://github.com/user-attachments/assets/f3f45903-70d3-4fb6-b7f2-bb3237b62d01)

![WhatsApp Image 2025-11-25 at 14 44 19_e326b44f](https://github.com/user-attachments/assets/426d8047-7883-41d4-939d-14eadbc49195)

![WhatsApp Image 2025-11-25 at 14 44 19_10ad3bbb](https://github.com/user-attachments/assets/bc0e132a-82ae-480a-b757-1a0b567ce469)


📝 Usage
Roles:
Admin: Manage all users, shelters, and pets

Shelter: Add/manage pets, respond to requests

Adopter: Search pets, request adoption

Authentication:
Register and login according to role

Role-based dashboard is displayed upon login

🩹 Troubleshooting
Common Issues:

404 on dashboard JSPs:
Make sure all .jsp files are included in the WAR and deployed to Tomcat.
Avoid naming conflicts (never use loop variable request in JSPs).

JSP compile errors:
See Tomcat logs for stack traces; resolve variable shadowing and uncaught exceptions.

Database errors:
Make sure MySQL server is running. Check credentials/config in DAO classes.

Session not working:
Ensure correct attribute names (userId, userRole, etc.).

Debug Tips:

Try direct access of JSPs to isolate deployment issues

Print session variables at top of each dashboard JSP for testing

💡 Contributing
Pull requests welcome! Fork the repo and submit features, bug fixes, or UI improvements.

📄 License
MIT License. See LICENSE for details.

🙋‍♂️ Author
Piyush Samal
