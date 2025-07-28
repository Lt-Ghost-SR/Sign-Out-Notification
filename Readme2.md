# 🪟 Custom Clock-Out Notification (Tkinter GUI)

A sleek, animated, and borderless **clock-out reminder** built with Python's Tkinter and Pillow libraries. This lightweight tool provides a visually appealing, smooth pop-up notification reminding you it's time to clock out—ideal for remote work, freelancers, or daily wrap-up routines.

---

## 📌 Features

- ✅ **Borderless GUI** with transparent background
- ✅ **Smooth animations** (fade-in & slide-up)
- ✅ **Timed alerts**: 
  - **Exact Out** = `Now + 5 minutes`
  - **Safe Out** = `Exact Out + 3 minutes`
- ✅ **System sound** using `winsound.MessageBeep()`
- ✅ **Custom icon** support (via Pillow)
- ✅ Can be scheduled via **Task Scheduler** or cron (Windows)

---

## 🧠 How It Works

1. The **Signout Launcher** schedules this script at a defined **Notification Time**.
2. When the script runs:
   - It calculates:
     - `Exact Out`: current time + 5 minutes
     - `Safe Out`: `Exact Out` + 3 minutes
   - A borderless window **fades in** and **slides up** from the bottom of your screen.
   - A subtle **system notification sound** is played.
3. The GUI remains visible for a limited time, then fades out or closes automatically.

---