# 🐧 Linux User Management Console

A web-based **Linux User Management Console** that provides an interactive and user-friendly interface for simulating common Linux user and group management commands.

The application converts traditional Linux administration commands into an easy-to-use graphical interface where users can manage users, groups, passwords, account settings, and login sessions.

---

## 📌 Project Overview

Managing Linux users and groups normally requires working with terminal commands such as `useradd`, `usermod`, `passwd`, `userdel`, and `groupadd`.

This project provides a **graphical Linux-style administration console** that makes these operations easier to understand and interact with.

The application includes a dashboard, user management, group management, command simulator, terminal output, and login/session information.

> **Note:** This is a browser-based simulation. The commands displayed by the application do not modify the actual users or groups of the computer on which the browser is running.

---

## ✨ Features

### 👤 User Management

* View all system users
* Add new users
* Modify existing users
* Delete users
* View UID and GID
* View home directories
* View login shells
* View user groups
* Activate or lock user accounts
* Search users

### 🔐 Password Management

* Change user passwords
* Lock user accounts
* Unlock user accounts
* Expire passwords
* Display password-related command output

### 👥 Group Management

* Create new groups
* View existing groups
* View group members
* Assign users to groups
* Display group information

### 💻 Linux Command Simulator

The application provides interactive simulations for commonly used Linux commands:

```bash
useradd
passwd
usermod
userdel
groupadd
groups
id
who
```

### 🖥️ Terminal Console

A terminal-style interface displays the commands and simulated results, helping users understand how Linux administration commands work.

### 📊 Dashboard

The dashboard provides an overview of:

* Total users
* Active users
* Locked users
* Total groups
* Recent activity
* Quick command actions

### 💾 Local Storage

User and group information can be stored using the browser's **LocalStorage**, allowing data to remain available after refreshing the page.

### 📱 Responsive Interface

The application is designed to work on:

* Desktop
* Laptop
* Tablet
* Smaller screens

---

## 🛠️ Technologies Used

| Technology   | Purpose                            |
| ------------ | ---------------------------------- |
| HTML5        | Application structure              |
| CSS3         | UI design and responsive layout    |
| JavaScript   | Application logic and interactions |
| LocalStorage | Browser-based data persistence     |
| Font/Icons   | User interface elements            |

---

## 📂 Project Structure

```text
IT-PROJECT/
│
├── IT-PROJECT-MODIFIED.html
└── README.md
```

The application is implemented as a **single HTML file**, containing the required HTML, CSS, and JavaScript.

---

## 🚀 How to Run

### Method 1 – Directly in Browser

1. Download or extract the project.
2. Locate:

```text
IT-PROJECT-MODIFIED.html
```

3. Double-click the file.
4. It will open in your default web browser.
5. The application is ready to use.

### Method 2 – Using VS Code

1. Open the project folder in **Visual Studio Code**.
2. Open `IT-PROJECT-MODIFIED.html`.
3. Install the **Live Server** extension if required.
4. Right-click the HTML file.
5. Select **Open with Live Server**.
6. The application will open in your browser.

---

## 🧭 Application Modules

### 1. Dashboard

The dashboard provides a quick overview of the current simulated Linux environment.

It displays statistics such as:

```text
Total Users
Active Users
Locked Users
Total Groups
```

---

### 2. Users

The Users module displays user information in a table.

Typical information includes:

```text
Username
Full Name
UID
GID
Home Directory
Shell
Status
Groups
```

Users can also be searched and managed from this section.

---

### 3. Add User

The Add User module allows administrators to create a simulated Linux account.

Example:

```bash
useradd -m -s /bin/bash john
```

The application updates the user list and displays the corresponding command/output.

---

### 4. Password Management

The password module simulates commands such as:

```bash
passwd username
passwd -l username
passwd -u username
passwd -e username
```

These commands represent:

* Changing a password
* Locking an account
* Unlocking an account
* Expiring a password

---

### 5. Modify User

The user modification module can simulate changes such as:

* Full name
* Home directory
* Login shell
* UID
* Groups
* Account status

Example:

```bash
usermod -s /bin/bash username
```

---

### 6. Delete User

Users can be removed from the simulated environment.

Example:

```bash
userdel username
```

The application updates the dashboard and user table after deletion.

---

### 7. Groups

The Groups module displays available Linux groups and their members.

Example:

```bash
groups username
```

and:

```bash
groupadd developers
```

---

### 8. User Information

The application simulates the Linux `id` command.

Example:

```bash
id username
```

Output may contain:

```text
uid=1001(username)
gid=1001(username)
groups=1001(username),27(sudo)
```

---

### 9. Login Sessions

The `who` command is represented through the session interface.

Example:

```bash
who
```

It can display simulated information such as:

```text
username   tty1   login time
```

---

### 10. Terminal

The terminal provides a Linux-inspired command-line interface.

Example:

```text
$ useradd -m student
useradd: user 'student' created successfully

$ id student
uid=1001(student) gid=1001(student) groups=1001(student)
```

This helps students understand the relationship between the GUI operations and Linux commands.

---

## 🔒 Security Note

This project is designed primarily for **educational and demonstration purposes**.

It does not directly execute Linux commands on the host operating system.

The password and account information entered into the browser should therefore be treated as **simulation data only**.

For a real production Linux administration system, authentication, authorization, secure password hashing, backend APIs, audit logging, and operating-system-level permissions would be required.

---

## 🎯 Objectives

The main objectives of this project are:

1. To provide a simple interface for understanding Linux user management.
2. To demonstrate commonly used Linux user and group commands.
3. To reduce the complexity of learning terminal-based administration.
4. To provide an interactive simulation of Linux administration tasks.
5. To help students understand user IDs, groups, permissions, and login sessions.
6. To demonstrate web-based implementation using HTML, CSS, and JavaScript.

---

## 🎓 Educational Use

This project can be used as a learning tool for topics related to:

* Linux Administration
* Operating Systems
* System Administration
* User and Group Management
* Shell Commands
* Web Technologies
* Frontend Development

---

## 🔮 Future Enhancements

The project can be extended with:

* Real Linux backend integration
* User authentication and administrator login
* MySQL/PostgreSQL database
* Role-based access control
* Real-time system monitoring
* File permission management
* Sudo privilege management
* SSH session management
* Activity/audit logs
* User profile management
* REST API integration
* Docker deployment
* Cloud hosting

---

## ⚠️ Limitations

* The current application is a browser-based simulation.
* Linux commands are not actually executed on the host machine.
* Data is stored locally in the browser.
* It does not provide real operating-system-level user management.
* It is not intended for production server administration.

---

## 📄 License

This project is intended for **educational and academic purposes**.

You may modify and extend the project for learning, demonstration, and college project requirements.

---

## 👨‍💻 Project Summary

**Linux User Management Console** provides a graphical representation of Linux user and group administration.

Instead of requiring users to remember multiple terminal commands, the application provides an interactive dashboard where they can perform simulated operations such as creating users, modifying accounts, managing passwords, creating groups, viewing user information, and checking login sessions.

The project combines **HTML, CSS, and JavaScript** to create a simple, responsive, and interactive Linux administration environment.
