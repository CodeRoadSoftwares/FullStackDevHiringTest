# 🏆 Smart Auto-Scheduling System for Employee Shifts  

## 📖 Overview  
This is a **dynamic** Employee Shift Management System where employees can **set their availability**, and an **automated scheduling system** will generate **optimized shifts** based on strict constraints.  

The system **dynamically adjusts schedules** when employees update their preferences while ensuring **fairness, efficiency, and compliance with work rules**.  

🚀 This is NOT a simple CRUD app—this requires **serious logic and optimization skills**.  

---

## 📌 Features  

### 🏢 **Employee Portal**  (Simple 1-2 page dashboard)
✅ **User Authentication** (Sign up & Log in)  
✅ **Set Availability** (User should be able to set:)  
   - **Preferred shifts** (Morning / Afternoon / Night) for each day of the week  
   - **Max working hours per week they'll work** (Must be within a system-defined minimum and maximum limit)  
   - **Days off** (Specify which days they won't work, an array with days will work)

✅ **View Assigned Shifts** (Updated dynamically based on availability & system constraints)  
✅ **Update Availability Anytime** (Triggers recalculation of shift schedules)  
✅ **Receive Notification if Preferences Cannot Be Fully Met** (Showing a simple text will also work)  

### 👑 **Admin Portal**  (Simple 1-2 page dashboard)
✅ **Manage Employee Seniority Levels (Junior, Mid-Level, Senior)**  
✅ **Define Minimum and Maximum Employees Per Shift** (A default value by system will also work)

### ⚡ **Automated Shift Scheduling System (Core Challenge)**  
Once employees submit their availability, the system must:  

✅ **Generate an optimized weekly schedule** while ensuring:  
   - At least **one senior employee per shift**  
   - **No single employee works consecutive shifts longer than 8 hours**  
   - **Each employee must have a minimum 12-hour gap between assigned shifts**  
   - **Max 5 shifts per week** per employee  
   - The system should **not understaff shifts unnecessarily**—as many employees as possible should be assigned in a shift to keep them working, while respecting constraints.  
   - Cannot exceed the **maximum number of employees per shift** (predefined by the system or admin).  
   - **Fair distribution of shifts** (no one gets all night shifts)

✅ **Dynamically adjust schedules** when an employee updates:  
   - **Preferred shifts**  
   - **Max working hours per week**  
   - **Days off**  

✅ **Recalculate and adjust shifts for other employees if necessary**  
✅ **Ensure no shifts are left unfilled if possible while maintaining constraints**  
✅ **Notify employees if their preferred choices cannot be fully met (A simple text in dashboard will work)**  

---

## ❌ What NOT to Do
- ❌ No brute-force or inefficient scheduling algorithms
- ❌ No static/predefined shift assignments (everything must be dynamic)
- ❌ No skipping the auto-adjustments logic

---

## 🛠 Tech Stack  
- **Backend:** Node.js (Express)
- **Database:** MongoDB
- **Frontend:** React
- **Authentication:** JWT
- **Scheduling Logic:** You decide. Your approach to solving the scheduling challenge will be the key factor in evaluating your solution.

---

## 🚀 Challenge Breakdown  
This system requires deep problem-solving skills and involves:  
✅ A **simple frontend** to interact with the system  
✅ A straightforward yet functional **authentication system**  
✅ **Advanced scheduling logic** to manage multiple constraints dynamically  
✅ **Efficient shift allocation** to balance fairness and availability    

---

## 📌 Submission Guidelines  
1. Implement your solution.  
2. **Write a clear README** explaining:  
   - Your **approach to solving the problem**  
   - Challenges faced & how you tackled them  
   - Future improvements you would suggest
   - Include a short demo video (optional but recommended)
3. **Push the code to GitHub** and submit the repository link to hr@coderoad.in.  
4. If applicable, deploy a **working demo** (Vercel for frontend, Render for backend).  

