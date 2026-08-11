# Smart Solar Energy Dashboard ⚡

A lightweight, full-stack web application featuring a native **C++ HTTP backend server** paired with a modern **HTML5/CSS3 frontend dashboard**.

> 📌 **Learning Project Note:** This project was created while learning Git and GitHub version control, C++ low-level socket programming, and full-stack web architecture.

---

## 📖 Project Overview

The **Smart Solar Energy Dashboard** simulates a real-time monitoring system for an off-grid solar installation.

Rather than using heavy third-party web frameworks, the backend is built from scratch in **C++** using Windows Sockets (`winsock2.h`). It runs a local HTTP web server on port `8080` that serves static web files (`index.html`, `style.css`) and handles a dynamic REST API endpoint (`/api/data`) to deliver live JSON sensor metrics (solar panel power output, battery charge level, and system status).

---

## ✨ Key Features

* **Native C++ Web Server:** Custom HTTP server handling TCP socket connections, HTTP headers, and file streams directly from disk.
* **Dynamic API Endpoint:** Generates live simulated telemetry data formatted as JSON on `/api/data`.
* **Modern UI/UX:** Clean, dark-mode glassmorphism dashboard styled with custom CSS.
* **Asynchronous Requests:** Uses vanilla JavaScript `fetch()` to pull metrics from the C++ backend without reloading the page.
* **Zero External Dependencies:** Built with standard C++ standard libraries and native Windows Sockets (`ws2_32`).

---

## 🛠️ Tech Stack

* **Backend:** C++ (GCC/MinGW, `winsock2.h` Sockets)
* **Frontend:** HTML5, CSS3, JavaScript (`fetch` API)
* **Tools & Control:** Git, GitHub, VS Code, Git Bash

---

## 📁 Repository Structure

```text
Solar_Project/
├── Server.cpp    # C++ HTTP web server & socket connection logic
├── index.html    # Frontend layout & async fetch script
├── style.css     # Responsive dark-theme styling
└── README.md     # Project documentation
