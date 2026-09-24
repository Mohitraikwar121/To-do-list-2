<div align="center">       
# 📝 To-Do List Application
### **One task at a time. One step closer to your goals.**

A modern, responsive, and lightweight **To-Do List web application** for creating, organizing, tracking, and managing everyday tasks directly in your browser.

Built with **HTML5, CSS3, and JavaScript**, the application requires **no backend, database, framework, or build process**.
 
<p> 
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5">
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3">
  <img src="https://img.shields.io/badge/JavaScript-ES6%2B-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript">
  <img src="https://img.shields.io/badge/LocalStorage-API-4CAF50?style=for-the-badge" alt="LocalStorage">
</p>

<p>
  <img src="https://img.shields.io/badge/Backend-None-lightgrey?style=flat-square" alt="Backend">
  <img src="https://img.shields.io/badge/Database-None-lightgrey?style=flat-square" alt="Database">
  <img src="https://img.shields.io/badge/Responsive-Yes-0A66C2?style=flat-square" alt="Responsive">
  <img src="https://img.shields.io/badge/Offline-Supported-2E7D32?style=flat-square" alt="Offline">
  <img src="https://img.shields.io/badge/License-Educational-green?style=flat-square" alt="License">
</p>

**[Features](#-features) • [Architecture](#-architecture) • [Getting Started](#-getting-started) • [Usage](#-usage) • [Project Structure](#-project-structure) • [Roadmap](#-roadmap) • [Contributing](#-contributing)**

</div>

---

## 📌 Overview

The **To-Do List Application** is a client-side task management application designed to provide a simple and distraction-free workspace for managing everyday tasks.

Users can create, edit, complete, delete, and filter tasks while their data is automatically persisted in the browser using the **LocalStorage API**.

### 🎯 Core Principles

| Principle             | Description                                                        |
| --------------------- | ------------------------------------------------------------------ |
| 🎯 **Simplicity**     | Keep task management quick, clear, and clutter-free                |
| ⚡ **Efficiency**      | Make common task operations accessible with minimal interaction    |
| 📱 **Responsiveness** | Provide a consistent experience across desktop, tablet, and mobile |
| 💾 **Persistence**    | Preserve tasks across page refreshes and browser sessions          |

> **Architecture:** 100% client-side — no backend server, database, or build process is required.

---

# ✨ Features

## 📋 Task Management

| Feature              | Description                                             |
| -------------------- | ------------------------------------------------------- |
| ➕ **Create Tasks**   | Add a task with a title and optional description        |
| ✏️ **Edit Tasks**    | Modify existing task information                        |
| ✅ **Complete Tasks** | Mark tasks as completed or return them to active status |
| 🗑️ **Delete Tasks** | Permanently remove tasks                                |
| 📋 **Task Overview** | Manage all tasks from a centralized interface           |

---

## 🔎 Task Filtering

Quickly organize tasks according to their current status:

* **All** — Display every task
* **Active** — Display pending tasks
* **Completed** — Display finished tasks

---

## 💾 Local Data Persistence

Tasks are stored using the browser's **LocalStorage API**.

Your tasks remain available after:

* 🔄 Refreshing the page
* 🌐 Closing and reopening the browser
* ↩️ Returning to the application later

### ⚠️ Storage Limitation

LocalStorage is **browser/device-specific**.

Therefore:

* ❌ No cloud synchronization
* ❌ No multi-device synchronization
* ❌ No user accounts
* ❌ No server-side storage

Clearing the browser's site data or LocalStorage can remove saved tasks.

---

## 📱 Responsive Design

The interface is designed to work across:

**🖥️ Desktop · 💻 Laptop · 📱 Tablet · 📲 Mobile**

The layout, spacing, typography, and controls adapt to different screen sizes while maintaining usability.

---

# 🛠️ Technical Highlights

* Modular frontend structure
* Client-side application state management
* Dynamic DOM rendering
* CRUD-style task operations
* LocalStorage persistence
* Real-time UI updates
* Status-based task filtering
* Event-driven interactions
* Form validation and input handling
* Responsive CSS layout
* Mobile-friendly interface
* No framework dependency
* No build tools required
* No backend or database required

---

# 💻 Technology Stack

| Technology            | Purpose                                                                 |
| --------------------- | ----------------------------------------------------------------------- |
| **HTML5**             | Semantic application structure and UI markup                            |
| **CSS3**              | Styling, responsive layout, spacing, and presentation                   |
| **JavaScript (ES6+)** | Application logic, state management, DOM manipulation, and interactions |
| **LocalStorage API**  | Persistent client-side task storage                                     |



# 🏗️ Architecture

The application follows a simple client-side architecture:


                    ┌─────────────────────┐
                    │     User Interface  │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │     HTML + CSS      │
                    └──────────┬──────────┘
                               │
                               ▼
                 ┌───────────────────────────┐
                 │   JavaScript Application   │
                 │          Logic             │
                 └────────────┬──────────────┘
                              │
          ┌───────────────────┼────────────────────┐
          │                   │                    │
          ▼                   ▼                    ▼
   Task Creation       Task Management      Task Filtering
          │                   │                    │
          └───────────────────┼────────────────────┘
                              │
                              ▼
                    ┌─────────────────────┐
                    │   LocalStorage API  │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │   Browser Storage   │
                    └─────────────────────┘




# 🔄 Application Workflow


             ┌──────────────────┐
             │   Create Task    │
             └────────┬─────────┘
                      │
                      ▼
             ┌──────────────────┐
             │   Active Task    │
             └────────┬─────────┘
                      │
            ┌─────────┴─────────┐
            ▼                   ▼
     ┌──────────────┐    ┌──────────────┐
     │  Edit Task   │    │ Delete Task  │
     └──────┬───────┘    └──────────────┘
            │
            ▼
     ┌──────────────┐
     │ Save Changes │
     └──────┬───────┘
            │
            ▼
     ┌──────────────────┐
     │ Mark Completed   │
     └────────┬─────────┘
              │
              ▼
     ┌──────────────────┐
     │ Completed Task   │
     └──────────────────┘


# 💾 Data Persistence

Whenever a user creates, updates, completes, or deletes a task, the application updates the stored task data.

On application startup, previously stored tasks are retrieved from LocalStorage and rendered in the interface.

### Persistence Flow

User Action
     │
     ▼
Application State
     │
     ▼
LocalStorage
     │
     ▼
Browser Storage

### Storage Characteristics

| Property          | Value                |
| ----------------- | -------------------- |
| Storage           | Browser LocalStorage |
| Persistence       | ✅ Yes                |
| Backend           | ❌ None               |
| Database          | ❌ None               |
| Cloud Sync        | ❌ No                 |
| Multi-device Sync | ❌ No                 |
| Data Scope        | Browser / Device     |


# 🗂️ Project Structure

To-Do-List/
│
├── index.html
├── style.css
├── script.js
│
├── screenshots/
│   ├── home.png
│   ├── add-task.png
│   ├── edit-task.png
│   └── completed-tasks.png
│
└── README.md

### 📄 File Responsibilities

| File / Directory | Responsibility                                                     |
| ---------------- | ------------------------------------------------------------------ |
| `index.html`     | Application structure and UI elements                              |
| `style.css`      | Styling, layout, and responsive design                             |
| `script.js`      | Task logic, event handling, filtering, and LocalStorage operations |
| `screenshots/`   | Screenshots used for project documentation                         |
| `README.md`      | Project documentation                                              |


# 🚀 Getting Started

## Prerequisites

Only a few things are required:

* A modern web browser
* A code editor such as **Visual Studio Code**
* Git *(optional)*

No backend server, database, package manager, or runtime environment is required.

## ▶️ Run Locally
### Option 1 — Open Directly

1. Download or clone the repository.
2. Open the project folder.
3. Double-click `index.html`.
4. The application will open in your browser.

### Option 2 — VS Code + Live Server

For a better development experience:

1. Open the project in **Visual Studio Code**.
2. Install the **Live Server** extension.
3. Right-click `index.html`.
4. Select **Open with Live Server**.
5. The application will open automatically in your browser.

# 📖 Usage
## ➕ Create a Task

1. Enter a task title.
2. Add an optional description.
3. Select **Add Task**.
4. The task appears in the task list.

## ✏️ Edit a Task

1. Locate the task.
2. Select **Edit**.
3. Modify the task details.
4. Save the changes.

## ✅ Complete a Task

Use the task checkbox/control to change its status between **Active** and **Completed**.

## 🗑️ Delete a Task

Select **Delete** to permanently remove the task.

## 🔎 Filter Tasks

Use the available filters to switch between:

* All
* Active
* Completed

# 🖼️ Screenshots
## 🏠 Dashboard

<img src="screenshots/home.png" alt="To-Do List Dashboard" width="800">

## ➕ Add Task

<img src="screenshots/add-task.png" alt="Add Task" width="800">

## ✏️ Edit Task

<img src="screenshots/edit-task.png" alt="Edit Task" width="800">

## ✅ Completed Tasks

<img src="screenshots/completed-tasks.png" alt="Completed Tasks" width="800">

# 🌐 Browser Support
| Browser           | Support |
| ----------------- | ------- |
| Chrome            | ✅       |
| Firefox           | ✅       |
| Edge              | ✅       |
| Safari            | ✅       |
| Opera             | ✅       |
| Internet Explorer | ❌       |

> The application requires a modern browser with LocalStorage support.

# 🎨 Design & User Experience
### 🎯 Simplicity

The interface minimizes unnecessary elements and keeps the primary task workflow easy to understand.

### 📱 Responsiveness

The layout adapts to different viewport sizes for a consistent desktop and mobile experience.

### ⚡ Efficiency

Common operations such as adding, completing, editing, deleting, and filtering tasks are available directly from the main interface.

### 👁️ Visual Hierarchy

Task titles, descriptions, completion states, and available actions are organized for quick scanning.

### ♿ Usability

Clear controls and predictable interactions help users manage tasks without unnecessary complexity.


# 🎯 Project Objectives
This project demonstrates practical frontend development concepts:

* Building a functional task-management application
* Implementing CRUD operations
* Managing client-side application state
* Working with the DOM
* Handling user interactions and events
* Implementing persistent browser storage
* Building responsive interfaces
* Implementing task filtering
* Handling form input and validation
* Organizing frontend code effectively
* Developing a practical real-world web application


# 🧠 Key Learning Outcomes
Through this project, the following concepts are demonstrated:

* JavaScript application logic
* DOM manipulation
* Event handling
* CRUD operations
* LocalStorage integration
* Data serialization and retrieval
* Client-side state management
* Conditional rendering
* Task filtering
* Form validation
* Responsive CSS
* User interaction design
* Frontend project organization

# 🗺️ Roadmap
Future improvements are planned in multiple phases.

## Phase 1 — Productivity

* [ ] Task priorities
* [ ] Due dates
* [ ] Reminders
* [ ] Categories and tags
* [ ] Task search
* [ ] Task sorting
* [ ] Drag-and-drop ordering

## Phase 2 — User Experience

* [ ] Dark / Light theme
* [ ] Browser notifications
* [ ] Advanced filtering
* [ ] Keyboard shortcuts
* [ ] Improved accessibility
* [ ] Better empty-state messages
* [ ] Improved mobile interactions

## Phase 3 — Full-Stack Expansion

* [ ] User authentication
* [ ] REST API integration
* [ ] Backend service
* [ ] Database integration
* [ ] Cloud synchronization
* [ ] Multi-device access
* [ ] User-specific task management
* [ ] Collaborative task management


# ❓ FAQ
### Will I lose my tasks if I clear my browser data?

Yes. Tasks are stored in LocalStorage, so clearing the application's site data can remove them.

An export/backup feature is planned for a future version.

### Can I use the application on multiple devices?

Not currently.

Tasks are stored locally in the browser and are not synchronized between devices.

Multi-device synchronization is planned as part of the future full-stack expansion.

### Does the application require an internet connection?

No.

Once the application is loaded, it can operate offline because the application logic runs entirely on the client side.

### Does the application require a backend?

No.

The current version does not use a backend server or database.

# 📊 Project Information
| Property             | Details                     |
| -------------------- | --------------------------- |
| **Project Name**     | To-Do List Application      |
| **Category**         | Web Development             |
| **Application Type** | Task Management             |
| **Architecture**     | Client-Side Web Application |
| **Frontend**         | HTML5, CSS3, JavaScript     |
| **Storage**          | Browser LocalStorage        |
| **Interface**        | Responsive Web UI           |
| **Backend**          | None                        |
| **Database**         | None                        |
| **Status**           | ✅ Completed                 |


# 🤝 Contributing
Contributions, improvements, and feature suggestions are welcome.

### Contribution Workflow

Fork Repository
       ↓
Create Feature Branch
       ↓
Implement Changes
       ↓
Test Changes
       ↓
Commit Changes
       ↓
Push Branch
       ↓
Open Pull Request


### Contribution Guidelines
* Keep changes focused on a specific feature or fix.
* Maintain the existing project structure and coding style.
* Ensure existing functionality continues to work.
* Test changes before submitting a pull request.
* Use clear and meaningful commit messages.

# 📄 License
This project is developed for **educational and portfolio purposes**.

You are free to modify, extend, and adapt the project for learning and development purposes.

# ⭐ Support

If this project helped you learn something new, consider giving it a ⭐ **Star** on GitHub.

Your support helps others discover the project and encourages further development.

<div align="center">

### 📝 Built to keep tasks simple, organized, and actionable.

**One task at a time. One step closer to your goals.**

</div>
