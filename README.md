# Task 2 - Servlet Based CRUD Application

## Contact Manager Module

This project implements Task 2 of the Java Full Stack Web Development internship.

### Objective
Transform a static personal portal into a dynamic contact management system using Java Servlets, JSP, JSTL and JavaBeans.

### Features
- `GET /contacts` - display all contacts
- `GET /contacts/add` - display add-contact form
- `POST /contacts` - validate and add a contact
- Server-side validation for name, email and phone
- Client-side real-time validation
- HTTP session based in-memory storage
- JSP + JSTL view layer
- Search-as-you-type
- Pagination
- Success/error alerts and toast
- Loading spinner
- Auto-focus first invalid field
- XSS-safe output using JSTL `<c:out>`
- Duplicate submission protection using a session form token

### Validation
- Name: required, 2-50 characters
- Email: required, valid email format
- Phone: optional, exactly 10 digits if provided

### Technology
- Java 11+
- Java Servlets 4
- JSP
- JSTL
- JavaBeans
- HTML5
- CSS3
- JavaScript
- Maven
- Apache Tomcat 9

### Important
The task specification says data is stored in-memory and database persistence is planned for Task 3. Therefore this implementation uses the HTTP session rather than MySQL.

## Run
1. Install JDK 11 or newer.
2. Install Maven.
3. Install Apache Tomcat 9.
4. Run:
   ```bash
   mvn clean package
   ```
5. Copy:
   `target/contact-manager.war`
   to Tomcat's `webapps` directory.
6. Start Tomcat.
7. Open:
   `http://localhost:8080/contact-manager/contacts`

## GitHub
```bash
git init
git add .
git commit -m "Complete Task 2 Contact Manager"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/task2-contact-manager.git
git push -u origin main
```

Replace `YOUR_USERNAME` with your GitHub username.
