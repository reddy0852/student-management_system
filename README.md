# Student Management System

This is a student management system that provides CRUD (Create, Read, Update, Delete) operations for student data through a REST API.

## Features

- Add new students
- View a list of students
- Update student information
- Delete students

## Usage

The system exposes the following endpoints:

- `GET /students` - Retrieves a list of all students
- `POST /students` - Creates a new student
- `GET /students/{id}` - Gets a specific student by id
- `PUT /students/{id}` - Updates a student
- `DELETE /students/{id}` - Deletes a student

### Sample Requests

**GET /students**

**POST /students**
```json
{
  "name": "John Doe",
  "email": "john@example.com"
}
```
**PUT /students/1**
```json
{
  "name": "Jane Doe"
}

```
##  Technologies
Java
Spring Boot - REST API framework
Apache Tomcat - Servlet container
MySQL - Database
Git - Version control
##  Installation
1. Clone the repository:
``` bash
git clone "https://github.com/reddy0852/student-management_system.git"
```

2.  Configure MySQL database connection in 
  'src/main/resources/application.properties'. 

3. Build using Maven:
```bash
mvn clean install
```
4. Deploy the generated WAR file to Apache Tomcat.

5. Access the API at http://localhost:8080/api/students.