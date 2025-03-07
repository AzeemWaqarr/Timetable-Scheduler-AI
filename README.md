# Timetable Scheduling using Genetic Algorithm 🧬

## 📌 Project Overview
This project implements an **AI-based timetable scheduling system** using a **Genetic Algorithm (GA)**. The algorithm optimizes course schedules while satisfying hard and soft constraints to minimize conflicts.

## 🛠️ Installation & Setup
### 1. Clone the Repository
```sh
git clone https://github.com/AzeemWaqarr/Timetable-Scheduler-AI.git
cd Timetable-Scheduler-AI
```

### 2. Install Dependencies
```sh
pip install -r requirements.txt  # (if applicable)
```

## 📂 Project Structure
```
📦 Timetable-Scheduler-AI
├── 📄 README.md       # Project Documentation
├── 📄 Project Report.pdf  # Detailed Report
├── 📄 AI Course Project - Timetable Scheduling.pdf  # Instructions
├── 📂 notebooks
│   ├── i210679_AI_Project.ipynb  # Jupyter Notebook with Implementation
└── 📂 data (if any datasets are used)
```

## 🎯 Genetic Algorithm Implementation
### **1️⃣ Chromosome Representation**
Each timetable is encoded as a **chromosome**, storing information such as:
- **Course & Type (Theory/Lab)**
- **Section & Section Strength**
- **Professor Assigned**
- **Time Slots & Rooms**

### **2️⃣ Fitness Function**
The **fitness function** evaluates schedule quality by penalizing conflicts:
✅ No professor teaches two classes at the same time.  
✅ No section is assigned multiple classes at the same time.  
✅ Room capacity constraints are respected.  
✅ Labs are scheduled in afternoon sessions.  
✅ Lecture days are spread out properly.  

### **3️⃣ Crossover & Mutation**
- **Crossover:** Two parent schedules exchange genetic material at a random point.  
- **Mutation:** Random changes ensure diversity in timetable generation.

### **4️⃣ Evolution Process**
- **Population Initialization:** A set of random schedules is generated.
- **Selection:** The best schedules are chosen for reproduction.
- **Crossover & Mutation:** The population evolves over **100 generations** to find the optimal timetable.

## 📊 Results & Performance
- The algorithm runs for **100 generations**, optimizing schedules.
- The **best timetable** is selected based on the **lowest conflict score**.
- Detailed results, visualizations, and analysis are available in the Jupyter Notebook.

## 📬 Contact
- **Email:** azeem.waqarr@gmail.com  
- **GitHub:** [AzeemWaqarr](https://github.com/AzeemWaqarr)  
