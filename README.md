# Zoom - Full Stack Video Conferencing Web Application

A comprehensive, full-stack video conferencing web application designed to facilitate seamless real-time virtual meetings. This project features a robust modern web architecture, offering secure user authentication, interactive meeting environments, and comprehensive meeting history tracking.

## 🚀 Features

### Core Functionality

* **Real-Time Video Meetings:** Live, interactive video conferencing capabilities powered by WebSockets.


* **User Authentication:** Secure sign-up, login, and session management system.


* **Meeting History Dashboard:** Dedicated interface for users to track, view, and manage past virtual meetings.


* **Instant Meeting Access:** Streamlined landing and home pages designed for rapid meeting creation and joining.



### Modern Interface Features

* **Responsive UI:** Clean, intuitive interface built with React.


* **Dedicated Video Component:** Modular and encapsulated video meeting interface (`VideoMeet.jsx`).


* **Protected Routes:** Context-aware routing that ensures only authenticated users can access specific application features (`withAuth.jsx`).



## 🛠️ Technology Stack

**Backend & Real-time Services**

* **Node.js:** Core backend runtime environment.


* **WebSockets:** Handles real-time bidirectional communication and video signaling (`socketManager.js`).


* **RESTful API:** Dedicated controllers and routes for user management (`user.controller.js`, `users.routes.js`).



**Database & Storage**

* **Database Models:** Structured schema models for managing Users and Meetings (`user.model.js`, `meeting.model.js`).



**Frontend**

* **React.js:** Component-based frontend architecture.


* **Context API:** Global state management for authentication and user sessions (`AuthContext.jsx`).


* **CSS Modules:** Scoped, component-specific styling (`videoComponent.module.css`).



## 📁 Project Architecture

**Backend Architecture:**
The server utilizes a modular structure separating configurations (`app.js`), business logic (`controllers/`), database schemas (`models/`), and API endpoints (`routes/`). Real-time meeting connections are strictly managed by a dedicated socket manager.

**Frontend Architecture:**
The client side is organized into distinct pages (`home.jsx`, `landing.jsx`, `history.jsx`, `authentication.jsx`) with reusable context providers and utility functions. Access to the core application is secured using higher-order authentication wrappers.
