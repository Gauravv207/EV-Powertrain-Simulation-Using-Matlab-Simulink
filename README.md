# EV-Powertrain-Simulation-Using-Matlab-Simulink

**Overview**
This project presents a basic simulation of an electric vehicle (EV) powertrain developed in MATLAB/Simulink (R2025b). The model is built without using Simscape Electrical or powergui blocks, and instead relies on fundamental Simulink components.
The objective is to study the interaction between the battery, motor, and vehicle dynamics, and to observe how input conditions affect vehicle speed, torque, and energy consumption.

**Model Description**

The system consists of the following main subsystems:
Battery (State of Charge based model)
Controller (driver input / throttle logic)
Motor (simplified torque-speed relation)
Vehicle dynamics (longitudinal motion)
Load forces (rolling resistance and aerodynamic drag)

**Simulink Model**

Complete Model
Battery and Controller Section
Motor Subsystem

**Sample Calculation**

Rolling resistance:
F_rolling = 1200 × 9.81 × 0.01
F_rolling = 117.72 N
Aerodynamic drag:
F_aero = 0.5 × 1.225 × 2.2 × 0.3 × (20)²
F_aero ≈ 323.4 N
Total force (neglecting gradient and acceleration):
F_total ≈ 117.72 + 323.4
F_total ≈ 441.12 N

 
 Results and Interpretation

The simulation results illustrate the dynamic behavior of the electric vehicle system under the given operating conditions.

 State of Charge (SOC)

The blue curve represents the battery State of Charge (SOC). It starts at an initial value of 1 (i.e., 100%) and gradually decreases to approximately 0.75 over the simulation period. This indicates continuous battery discharge as energy is supplied to the motor. The decreasing trend validates that the model correctly captures energy consumption during vehicle operation.

 Vehicle Speed

The yellow curve represents the vehicle speed. It shows a smooth and gradual increase over time, indicating acceleration of the vehicle in response to the applied throttle input. The absence of instability or abrupt changes confirms proper functioning of the control and motor dynamics.



<img width="1920" height="1020" alt="Scope Output Waves" src="https://github.com/user-attachments/assets/8749055b-56db-4f17-a60d-27559eafeb60" />













