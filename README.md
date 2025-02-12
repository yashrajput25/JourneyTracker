# Journey Tracker App

## 📌 Overview
The **Journey Tracker App** allows users to track their journey with multiple stops, displaying:
- **Current stop name**
- **Distance to the next stop (in km or miles, with a toggle button)**
- **Progress bar to show journey completion**
- **List of stops, dynamically updated as the journey progresses**
- **User interaction with buttons to toggle distance units and move to the next stop**

This app is implemented using **two versions:**
1. **Jetpack Compose Version** (Modern UI with Compose)
2. **Traditional XML + Kotlin Version** (Using `RecyclerView` and `ProgressBar`)

---

## 📂 Project Structure
```
app/
│-- src/
│   ├── main/
│   │   ├── java/com/example/journeytracker/
│   │   │   ├── MainActivity.kt   # Traditional XML + Kotlin Version
│   │   │   ├── StopsAdapter.kt   # RecyclerView Adapter for XML Version
│   │   │   ├── MainActivity.kt   # Jetpack Compose Version
│   │   ├── res/
│   │   │   ├── layout/
│   │   │   │   ├── activity_main.xml   # XML Layout for Traditional Version
│   │   │   │   ├── item_stop.xml       # XML Layout for RecyclerView Items
│   │   │   ├── raw/
│   │   │   │   ├── stops.txt           # File containing stops and distances
```

---

## 🚀 Features
✅ **Dynamic Stop Loading:** Reads stops and distances from `stops.txt`
✅ **Displays Next Stop Distance:** Automatically updates on reaching a new stop
✅ **Progress Bar:** Updates journey progress
✅ **Toggle Between KM and Miles:** Allows users to switch distance units
✅ **Scrollable List of Stops:** Uses `LazyColumn` in Compose and `RecyclerView` in XML version
✅ **Disabled Button at Last Stop:** Prevents clicking "Next Stop" after final destination

---

## 🛠️ Dependencies
- **Jetpack Compose (for Compose version)**
- **Material3 Components (Buttons, Progress Bar, Divider, etc.)**
- **RecyclerView & LinearLayoutManager (for XML version)**

---

## 📜 How to Use
### 1️⃣ **Jetpack Compose Version**
1. **Load stops and distances from `stops.txt`** in `res/raw/`
2. **Toggle Distance Button** - Converts between KM and Miles
3. **Click "Next Stop Reached"** to move to the next stop
4. **Progress Bar Updates** dynamically
5. **Stops List Grows Dynamically** using `LazyColumn`

### 2️⃣ **XML + Kotlin Version**
1. **RecyclerView** displays reached stops dynamically
2. **Progress Bar updates** as journey progresses
3. **Buttons to Toggle Distance and Reach Next Stop**

---

## 📂 `stops.txt` Format
```
New York, 200
London, 250
Dubai, 300
Delhi, 150
Sydney, 0
```
✅ **First column** = Stop Name  
✅ **Second column** = Distance to the next stop (in km)

---

## 📦 How to Run the Project
### **1️⃣ Clone the Repository**
```bash
git clone <your-repo-url>
```

### **2️⃣ Open in Android Studio**
- Open the project in **Android Studio**
- Select **Run** ▶ to launch on an emulator or physical device

---


## 📜 License
This project is **free to use** for learning purposes.

🚀 **Happy Coding!**

