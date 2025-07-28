# ⏳ Work Session Sign-Out-Notification

A lightweight, two-part toolset designed to manage your work sessions effectively with start-time logging, end-of-day reminders, and a beautifully animated GUI clock-out notification.

---

## 🧩 What's Included

1. 🖥️ **Sign-Out Scheduler (Console App)**  
   A terminal-based utility that logs your work session, calculates your out time, and schedules a reminder.  
   ❗ **Note:** The default work duration is set to **8 hours and 30 minutes**.

2. 🪟 **Clock-Out Notification (Tkinter GUI)**  
   A sleek, borderless, animated popup reminder built with Tkinter and Pillow that notifies you when it's time to clock out.  
   ✅ You can replace this with your own custom notification `.exe` file via the Signout Scheduler Menu.

3. 🔐 **User Configuration Storage**  
   This repository contains a `user_data.json` file that saves your username and the path to your sign-out notification `.exe` file, ensuring your preferences persist between sessions.

---

## 📦 Features

### ✅ Common Features
- Auto-schedules a **Task Scheduler** job based on your session timing
- User-friendly, customizable experience
- Designed for **Windows** environments

### 🖥️ Sign-Out Scheduler (Console)
- 📝 Configure your notification `.exe` path
- 👤 Personalize with your user name
- ⏰ Uses **system boot time** or manual input as clock-in time
- 📅 Calculates:
  - **Notification Time**
  - **Exact Out Time** (5 minutes after notification)
  - **Safe Out Time** (3 minutes after out time)
- 🧠 Auto-creates a Task Scheduler job

### 🪟 Clock-Out Notification (GUI)
A clean, borderless pop-up appears 5mins before Exaact out, with:
- ✅ Motivational header: Great Work Today!
- ⏰ Displays timing: **Exact Out** and **Safe Out**
- 💬 Friendly message: "Please sign out at your convenience."

---

## 🚀 Getting Started

1. Clone or download this repository.
2. Unzip the file and locate `Scheduler Terminal.exe`.
3. Create a shortcut for this `.exe` file.
4. Paste the shortcut into the **Startup Apps** folder to launch it automatically at system boot:

   - Press `Win + R` to open the **Run** dialog.
   - Type: `shell:startup`
   - Press Enter.
   - Paste the shortcut into the folder that opens.

5. After the `.exe` file starts, the **Command Terminal Interface** will appear.
6. Configure **Option [1]** – Navigate to and select your `Notification.exe` (or any notification app you want to use).
7. Configure **Option [2]** – Change the name displayed in the terminal (for personalization).
8. To use the **system boot time** automatically, just press **Enter** when prompted.  
   Or, enter your manual boot/signed-in time in `HH:MM` (24-hour format).
9. It calculates and schedules your notification task.

<img width="648" height="264" alt="image" src="https://github.com/user-attachments/assets/a345231c-6c3b-4435-ac79-f378a09463f3" />

📅 **Example Output**

Boot Date: `2025-07-27` | Boot Time: `08:00:00`

Notification: `16:25:00`
Out time: `16:30:00`
Safe Out: `16:33:00`

Task scheduled successfully at `16:30`

## 🧠 Custom Signout Notification

1. The **Signout Launcher** schedules this script at a defined **Notification Time**.
2. When the script runs:
   - It calculates:
     - `Exact Out`: current time + 5 minutes
     - `Safe Out`: `Exact Out` + 3 minutes
   - A borderless window **fades in** and **slides up** from the bottom of your screen.
   - A subtle **system notification sound** is played.
3. The GUI remains visible until the close button pressed.
<img width="350" height="180" alt="image" src="https://github.com/user-attachments/assets/6ab51305-d530-468d-95ea-eda85e80cd7a" />

---
