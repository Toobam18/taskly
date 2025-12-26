Taskly To-Do Manager 

Taskly is a lightweight task manager web app built with PHP, MySQL, HTML/CSS, and JavaScript. It includes secure authentication, a task dashboard with CRUD actions, filtering, and multiple ways to view tasks (Cards / Table / Calendar).

✨ Features:

- Authentication
    - User registration + login + logout
    - Passwords stored securely using `password_hash()` + verified with `password_verify()`
    - Session-based authentication (protected dashboard route)

- Task Management
    - Create / Edit / Delete / Complete tasks
    - Task fields include:
    - Title, description, due date, category, status, grading (optional)
  - Filter tasks by:
      - Category
      - Status (ex: all / completed / pending)

- Views
    - Cards view
    - Table view
    - Calendar view
    - Calendar navigation uses AJAX (no full-page refresh)

 🧰 Tech Stack

- Frontend: 
    - HTML
    - CSS 
    - JavaScript

- Backend:
    - PHP
    - Database: MySQL
    - Local dev: WAMP/XAMPP/MAMP (or any Apache + PHP + MySQL setup)
 
💡 Design Inspiration

Taskly was inspired by **my own custom Notion workspace**, which I built to manage
courses, exams, and assignments.

This workspace combined multiple views *Cards, Table, and Calendar) to visualize
tasks at different levels of detail. Because this personalized system proved highly effective
for my workflow, I reimplemented the same concepts from scratch in Taskly using
PHP, MySQL, and JavaScript.

This project does not replicate a built-in Notion feature, but rather translates a
custom productivity workflow into a standalone web application designed specifically
for students.

![Custom Notion Workflow Inspiration](assets/custom-notion-workflow.png)


📁 Project Structure

```txt
Taskly/
├── db.php              # MySQL connection
├── login.html          # Login UI
├── login.css           # Login styling
├── login.js            # Login validation + password reveal
├── login.php           # Login handler (session start)
├── register.html       # Registration UI
├── register.php        # Registration handler (+ AJAX email check)
├── logout.php          # Destroys session
├── tasks.php           # Main dashboard (CRUD, filters, views)
├── tasks.js            # Dashboard interactivity + AJAX calendar nav
├── tasks.css           # Dashboard styling
└── assets/             # (optional) screenshots, logos, flowchart
