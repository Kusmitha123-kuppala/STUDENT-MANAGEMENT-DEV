# 🎓 Student Management Web Application
A modern, DevOps-enabled **Student Management System** built using **Java Maven** with full integration of **Docker, GitHub, and Jenkins CI/CD**.  
This project demonstrates **end-to-end DevOps practices** along with a structured Java application.

---

## ✨ Features
👨‍🎓 Student Record Management: Add, view, update, and delete student details  
📋 Centralized Data Handling: Maintain student information in one place  
⚙️ Maven Build Automation: Dependency management and packaging  
🐳 Dockerized Application: Consistent and portable deployment  
🔄 CI/CD Pipeline: Automated build and deployment using Jenkins  
📦 GitHub Version Control: Source code tracking and collaboration  
⚡ Scalable & Lightweight: Industry-standard DevOps workflow  

---

## 🚀 Technologies Used

### Application Stack
- **Language**: Java  
- **Build Tool**: Maven  
- **Testing**: JUnit  

### DevOps Tools
- **Version Control**: Git & GitHub  
- **Containerization**: Docker  
- **CI/CD Automation**: Jenkins  

---

## 📋 Prerequisites
Ensure the following are installed on your system:

- Java JDK **11 or higher**
- Maven **3.6 or higher**
- Git
- Docker
- Jenkins

### Verify Installation
```bash
java -version
mvn -version
git --version
docker --version

🛠️ Installation & Setup
Clone the Repository
bash
Copy code
git clone https://github.com/your-username/student-management-system.git
cd student-management-system
Build the Project
bash
Copy code
mvn clean install
Run Unit Tests
bash
Copy code
mvn test

🐳 Docker Implementation
Build Docker Image
docker build -t student-management-app .
Run Docker Container
docker run -p 8080:8080 student-management-app

Open your browser and navigate to:

http://localhost:8080/login.html
🔄 Jenkins CI/CD Pipeline
This project uses Jenkins for Continuous Integration and Deployment.

Jenkins Pipeline Stages
GitHub Source Code Checkout

Maven Build & Test

Docker Image Creation

Application Deployment

Every code commit to GitHub automatically triggers the Jenkins pipeline.

📦 Project Structure
student-management-system/
├── pom.xml                 # Maven configuration
├── Dockerfile              # Docker build file
├── Jenkinsfile             # Jenkins CI/CD pipeline
├── src/
│   ├── main/
│   │   ├── java/           # Application source code
│   │   └── resources/
│   └── test/
│       └── java/           # JUnit test cases
└── README.md

🎯 Usage
Adding a Student
Enter student details (ID, Name, Department, etc.)
Click Add Student
Updating Student Details
Select a student record
Modify the required fields
Click Update Student
Deleting a Student
Select a student record
Click Delete Student
Confirm deletion
Viewing Students
Displays a list of all student records

🧪 Testing
Run all test cases:
mvn test

📝 Maven Commands

mvn clean	Remove target directory
mvn compile	Compile source code
mvn test	Run unit tests
mvn package	Package JAR/WAR
mvn install	Install to local repository
mvn clean install	Full Maven lifecycle

🔁 DevOps Workflow
Developer pushes code to GitHub
Jenkins automatically triggers the pipeline
Maven builds and tests the application
Docker creates the container image
Application is deployed automatically

📈 Future Enhancements
Kubernetes deployment
Cloud hosting (AWS / Azure)
Database integration
Role-based access control

👤 Author
Kusumitha Kuppala
B.Tech – Computer Science Engineering
Aspiring DevOps .

📄 License
This project is open source and available for educational use.

⭐ Conclusion
This Student Management System showcases how a Java application can be transformed into a DevOps-ready solution using Maven, Docker, GitHub, and Jenkins, following real-world industry practices.

Happy Learning & DevOps Automation! 🚀