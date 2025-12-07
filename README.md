# SrmMail (CCC Project 2)
### A Data Structures Driven Gmail Simulation

**SrmMail** is a comprehensive simulation of an email management system, demonstrating the practical application of Data Structures and Algorithms (DSA).

This project features a **hybrid interface system**:
1.  **Modern Web UI**: A responsive, Gmail-like graphical interface with sidebar navigation, composed emails, and reading panes.
2.  **CLI Terminal Mode**: A VS Code-styled command-line interface that mimics the original C++ backend logic.

---

## 🚀 Live Demo
You can view the live prototype here: **[GitHub Pages Link]** *(Enable via Settings > Pages)*

## 📂 Project Structure
*   **`index.html`**: Main application entry point.
*   **`js/`**: Contains core simulation logic (`simulation_logic.js`) and UI controllers.
*   **`css/`**: Styling for both the Web UI and the Terminal theme.
*   **`src/`**: Contains the original C++ source code (`messager.cpp`).

---

## 🛠 Core Data Structures (Backend Logic)
The core simulation logic (originally implemented in C++ and ported to JS) uses efficient data structures to manage high-volume email traffic:

### 1. User Accounts Management
*   **Doubly Linked List**: Utilized to efficiently manage the list of all user accounts.
*   **Features**:
    *   Create new accounts with unique usernames.
    *   Secure login authentication.
    *   O(n) traversal for user lookup.

### 2. Message Storage
*   **Singly Linked Lists**: Each user has two personal linked lists:
    *   `SentBox`: Stores sent messages.
    *   `Inbox`: Stores received messages.
*   **Message Node**: Each node contains sender, recipient, content, timestamp, and status flags (starred, read, deleted).

### 3. Message Retrieval & Search
*   **Vector (Dynamic Array)**: Used during search operations to store references to messages that match specific criteria (e.g., "From: Saurav").
*   **Algorithms**: Sequential search algorithms filter messages based on metadata and status.

---

## ✨ Features
### user Actions
*   **Authentication**: detailed Login/Signup system.
*   **Mode Switching**: Toggle seamlessly between "UI Mode" and "Terminal Mode" (Press `9` in CLI or the Toggle Button in UI).
*   **Persistence**: Session data is preserved when switching modes.

### Message Management
*   **Compose**: Send emails to other users (sanitized input).
*   **Inbox/Sent/Trash**: Organized folders for message management.
*   **Starring**: Mark important messages with a star.
*   **Deletion**: Move to Trash (soft delete) or permanently delete.
*   **Search**: Real-time filtering of messages by content or sender.

---

## 🎓 About This Project
This project was developed as **CCC Project 2** to demonstrate the effective utilization of:
*   **Graph/Linked List** for User Relationships.
*   **Queues/Lists** for Message Delivery.
*   **Frontend-Backend Integration** for seamless UX.

---
*Created by Sanjana*
