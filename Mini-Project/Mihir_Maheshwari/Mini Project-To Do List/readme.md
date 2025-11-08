# TODO App – Mini Project

This Mini Project is a simple TODO application, created as part of the Summer Mentorship Progamme (SMP) by the Exclusive club Institution of Engineers @ National Institute Of Technology Karnatak, Surathkal (IE@NITK). The TODO app lets users manage tasks by allowing them to add, update, check off, and delete items. The project demonstrates fundamental concepts of Java application development using a graphical user interface (GUI).

## Features

- **Add Tasks:** Easily add new tasks to your TODO list.
- **Mark Complete:** Check off tasks when they're done.
- **Edit Tasks:** Update details of existing tasks.
- **Delete Tasks:** Remove tasks that are no longer needed.
- **GUI Interface:** User-friendly interface built with Java Swing.
- **User Login System:** Register and login to manage tasks per user.
- **MySQL Database Integration:** Task details and user accounts are saved in a local MySQL database, enabling persistence and retrieval of task lists.

## Technology Stack

- **Java:** Main backend logic, object-oriented programming, event handling.
- **Java Swing:** Building the graphical user interface components such as buttons, tables, text areas, and dialog boxes.
- **JDBC (Java Database Connectivity):** Connecting, querying, and updating the MySQL database from the Java application.
- **MySQL:** Relational database used for storing users, tasks, task status, priority, creation dates, etc.

## Setup and Running

1. **Clone the Main SMP Repository**
   ```sh
   git clone https://github.com/Mihir3101/Java-AppProg-SMP-2020.git
   ```

2. **Navigate to the Mini Project Directory**
   ```sh
   cd Java-AppProg-SMP-2020/Mini-Project/Mihir_Maheshwari/Mini\ Project-To\ Do\ List
   ```

3. **Database Setup**
   - Install MySQL and create a database named `tododb`.
   - Create the required tables (`User`, `tasks`, and perhaps `priority` as referenced in code).
   - Update connection details if your MySQL password or username differs from `root` / `qwerty`.
   - Sample schema creation:
     ```sql
     CREATE DATABASE tododb;
     USE tododb;

     CREATE TABLE User (
       UserID VARCHAR(255) PRIMARY KEY,
       Name VARCHAR(255),
       DOJ DATE,
       Password VARCHAR(255)
     );

     CREATE TABLE tasks (
       UserID VARCHAR(255),
       Task VARCHAR(255),
       Description TEXT,
       Priority VARCHAR(20),
       Status BOOLEAN,
       DOC DATE,
       TaskID INT AUTO_INCREMENT PRIMARY KEY
     );
     /* Add 'priority' table if referenced */
     ```

4. **Open the Project in Your IDE**
   - Use any Java IDE (e.g., Eclipse, IntelliJ IDEA, NetBeans) and import the project.

5. **Compile and Run**
   - Build the project and run the main class (`todo.java`).

## Usage

- Launch the application.
- Register a new user or login as an existing user.
- Add your tasks in the input field and hit "Add".
- Click on tasks to mark them complete.
- Edit or delete tasks using the provided buttons in the dashboard.

<!--
## Screenshot

*Add a screenshot of your TODO app GUI here if available.*

## License

Distributed under the MIT License.
-->
---

**Project author:** Mihir3101
