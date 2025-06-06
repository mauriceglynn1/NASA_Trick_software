# 🚢 NASA Trick Submarine Simulation

This project uses [NASA Trick Simulation Toolkit](https://github.com/nasa/trick) to simulate submarine dynamics and display graphical results through a Java client.

---

## 🛠️ Requirements

Before running this simulation, ensure you have the following installed:

- [Trick Simulation Toolkit](https://github.com/nasa/trick)
- Python 3
- Java (JDK 8 or later)
- Maven
- g++ or clang++ compiler (for building the simulation)

---

## 📦 Repository Structure
NASA_Trick_software/
├── SIM_submarine/ # Trick simulation folder
│ └── S_main_* # Built Trick executable (after build)
├── RUN_test/ # Contains input.py (initial conditions, launch script)
├── models/ # Contains display model source code
│ └── graphics/
│ └── build/ # Will contain SubmarineDisplay.jar
└── Modified_data/ # Contains real-time setup Python

**How to run Simulation**

**Build the Simulation**
trick-CP
make

**Build Graphics Display**
cd models/graphics
mvn package
cd ../../../

**Running the Simulation
From the project root:**
./SIM_submarine/S_main_* RUN_test/input.py
