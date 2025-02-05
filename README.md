
# CPU Scheduling

This project implements various CPU scheduling algorithms, helping to understand and analyze their efficiency in different scenarios.

## Implemented Scheduling Algorithms

Out of the various CPU scheduling algorithms, I have implemented six specific ones:

### 1️⃣ First Come, First Served (FCFS)
- **Type:** Non-Preemptive  
- **Description:** Processes are executed in the order they arrive.  
- **Pros:** Simple and easy to implement.  
- **Cons:** Can lead to the **convoy effect**, increasing waiting time.

### 2️⃣ Shortest Job First (SJF)
- **Type:** Non-Preemptive  
- **Description:** The process with the shortest execution time is executed next.  
- **Pros:** Provides optimal average waiting time.  
- **Cons:** May cause **starvation** for longer processes.

### 3️⃣ Round Robin (RR)
- **Type:** Preemptive  
- **Description:** Each process gets a small unit of CPU time (time quantum), and if it doesn't complete, it goes to the end of the queue.  
- **Pros:** Fair to all processes and reduces response time.  
- **Cons:** Frequent **context switching** increases overhead.

### 4️⃣ Shortest Remaining Time First (SRTF)
- **Type:** Preemptive  
- **Description:** A preemptive version of SJF where the process with the shortest remaining burst time executes next.  
- **Pros:** Reduces waiting time and improves responsiveness.  
- **Cons:** **Frequent preemptions** can cause overhead.

### 5️⃣ Longest Remaining Time First (LRTF)
- **Type:** Preemptive  
- **Description:** A preemptive version where the process with the longest remaining burst time executes next.  
- **Pros:** Longer processes get CPU time sooner.  
- **Cons:** Can be inefficient if shorter jobs keep arriving.

### 6️⃣ Priority Scheduling
- **Type:** Preemptive / Non-Preemptive  
- **Description:** Processes are executed based on priority, with higher priority processes running first.  
- **Pros:** Ensures important tasks get executed sooner.  
- **Cons:** May cause **starvation** for lower-priority processes.

---

## 🔹 Features

✅ Takes process details (arrival time, burst time, priority, etc.) as input.  
✅ Computes key scheduling metrics:  
   - **Turnaround Time (TAT)**  
   - **Waiting Time (WT)**  
   - **Response Time (RT)**  
✅ Displays Gantt charts for visual representation of process execution.  
✅ Provides a performance comparison between different scheduling algorithms.  

---

## 🛠️ Technologies Used

- **Technologies Used**
+ JavaScript (55.9%)
+ HTML (28.7%)
+ CSS (15.4%)
- **Data Structures:** Queues, Priority Queues, and Arrays  
- **Graphical Representation:** ASCII-based Gantt charts or visualization using a plotting library  

---

## 📥 Installation & Usage

1. **Clone the Repository**  
   ```bash
   git clone https://github.com/your-username/cpu-scheduling.git
2.**Navigate to the Project Directory**

     ```bash
     git clone https://github.com/your-username/cpu-scheduling.git
   

3.**Compile & Run the Program**
    
    g++ scheduling.cpp -o scheduling
    ./scheduling
4.**Enter Process Details**
-Follow the on-screen instructions to input process details.
-Choose the desired scheduling algorithm to execute.

## 📌 Example Input
Enter number of processes: 4
Process | Arrival Time | Burst Time | Priority
P1      | 0           | 5          | 2
P2      | 1           | 3          | 1
P3      | 2           | 8          | 3
P4      | 3           | 6          | 2

## 📊 Example Output (Gantt Chart for FCFS)
Gantt Chart:
| P1 | P2 | P3 | P4 |
0    5    8    16   22  

Average Waiting Time: 5.5 ms
Average Turnaround Time: 10.5 ms

## 📜 License
This project is licensed under the MIT License - see the LICENSE file for details.

## 📩 Contact
For any queries or contributions, feel free to reach out to me:
📧 Email: Pratikshaparihar679@gmail.com
🔗 LinkedIn: http://www.linkedin.com/in/pratiksha033
🐙 GitHub: https://github.com/pratiksha033


