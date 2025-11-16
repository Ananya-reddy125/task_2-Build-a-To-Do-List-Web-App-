

# **Ultra App – Login, Dashboard, To-Do, Habits & Storage Manager**

This project is a **single-file front-end web application** built entirely with **HTML, CSS, and JavaScript**.
It includes a login screen, dashboard, to-do list manager, habit tracker, and a storage viewer.
All user data is stored using **browser localStorage**, so no backend is required.

---

## **✨ Features**

### **1. Login System**

* Saves username in `localStorage`
* Simple login → redirects user to dashboard
* Automatically loads saved username on next visit

### **2. To-Do List**

* Add new tasks
* Mark tasks as completed
* Delete tasks
* Tasks auto-saved in `localStorage`

### **3. Habit Tracker**

* Add new habits
* Track daily progress
* Increment/Reset day counter
* Delete habits
* All habits stored in `localStorage`

### **4. Storage Viewer**

* Shows all saved browser storage data:

  * User
  * Todos
  * Habits
* Helps with debugging and understanding saved data

### **5. Dark Mode**

* Toggle between **Light/Dark** themes
* Instant UI change
* (Customizable to save theme in localStorage)

---

## **📁 Project Structure**

```
UltraApp/
│
└── Iindex.html     (Main project file containing HTML + CSS + JavaScript)
```

*Everything (UI + Logic + Styles) is inside this one file.*

---

## **🚀 How to Run the Project**

### **Option 1 — Directly from Browser**

Just open:

```
Iindex.html
```

in any web browser (Chrome, Edge, Firefox, etc.)

---

### **Option 2 — Run with a Local Server (Recommended)**

Helps avoid CORS issues and ensures proper loading.

#### Using Python:

```
python -m http.server 8000
```

Then open:

```
http://localhost:8000/Iindex.html
```

---

## **🗄 Data Storage Details (localStorage)**

The app uses the following keys inside `localStorage`:

| Key      | Purpose                      |
| -------- | ---------------------------- |
| `user`   | Stores logged-in username    |
| `todos`  | Stores all to-do tasks       |
| `habits` | Stores habit list + progress |

✔ Data **remains even after page reload**
✔ Data persists until browser storage is cleared
✖ Not secure, do not store sensitive information

---

## **🎨 Customization Options**

* **Change background image**: modify CSS in `<style>` section
* **Persistent dark mode**: store theme value in `localStorage`
* **Data export/import**:

  * Convert todos & habits to JSON
  * Download or upload JSON file

---

## **⚠ Notes / Limitations**

* No backend server → everything runs in the browser
* Login is not secure (for demo only)
* Do not store passwords or personal data
* Works offline since everything is local

---

