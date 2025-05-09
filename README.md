`# ☁️ CloudSim SJF Scheduler Simulation

This project simulates a basic cloud computing environment using **CloudSim 4.0** with a custom scheduling algorithm: **Shortest Job First (SJF)**. It models datacenters, virtual machines, and cloudlets to demonstrate how tasks are executed using SJF in a virtual cloud setup.

---

## 📁 Project Structure

CloudSimProject/
├── src/
│ └── cloudsim/
│ ├── SJF_Scheduler.java
│ ├── DatacenterCreator.java
│ ├── SJFDatacenterBroker.java
│ ├── Constants.java
│ ├── GenerateMatrices.java
│ └── (any other helper classes)
├── lib/
│ ├── cloudsim-4.0.jar
│ └── cloudsim-examples.jar
├── bin/ ← created after compilation
└── .vscode/
└── settings.json ← Java classpath config for VS Code


---

## 🚀 How to Run This Project

### ✅ Prerequisites

- Java JDK 17 or above
- VS Code (or any Java IDE)
- Git (optional, for cloning)

### 🔧 Steps to Execute

1. **Clone the Repository**
   ```bash
   git clone https://github.com/AlgoAdept/CloudSimProject.git
   cd CloudSimProject
2. **Compile the code**
   javac -cp "lib/*" -d bin src/cloudsim/*.java
3. **Run the code**
   java -cp "bin;lib/*" cloudsim.SJF_Scheduler
The simulation displays:

Creation of datacenters and virtual machines

Cloudlet assignment using SJF

Execution timeline, start/finish/waiting times

Final Makespan (total time taken to complete all tasks)

🔎 What is CloudSim?
CloudSim is a Java-based simulation toolkit for modeling cloud environments and services. Developed by the CLOUDS Lab, it helps researchers and developers test scheduling, provisioning, and resource management without using real cloud infrastructure. It's widely used in academic research and prototyping cloud strategies.

📌 SJF Scheduler (Shortest Job First)
Greedy, non-preemptive algorithm

Prioritizes cloudlets with the shortest execution time

Minimizes average wait time

May lead to starvation for longer tasks if not handled with care
