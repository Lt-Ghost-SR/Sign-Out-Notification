# Work Session Sign-Out-Notification

A lightweight console-based application to log your work session start time, get notifications, and schedule end-of-day reminders.

---

## 📦 Features

- 📝 Update the path to your notification log file.
- 👤 Update your user name.
- ⏰ Automatically use system boot time as your clock-in time (or enter manually).
- 🛎️ Get notified before your session ends.
- 🧠 Scheduled task is created for end-of-session alert.
- 💖 Friendly and uplifting user interface.

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


## 💡 Usage Example

When you launch the app, you’ll see a menu:

================================================================================
MENU
---------------------------------
[1] | Update Notification File Path
[2] | Update User Name
[3] | Exit Program
================================================================================
You'll be prompted to enter your clock-in time or use the boot time.
The app will calculate:

Notification Time

Out Time

Safe Out Time

It then schedules a task based on the "Notification Time".

📅 Example Output

Boot Date: 2025-07-27 | Boot Time: 08:00:00

Notification: 16:25:00  
Out time:      16:30:00  
Safe Out:      16:33:00  

Task scheduled successfully at 16:30
