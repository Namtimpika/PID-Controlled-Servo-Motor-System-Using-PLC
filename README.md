# PID-Controlled-Servo-Motor-System-Using-PLC
-Overview
This project implements a PID controller for servo motor position control using a Siemens PLC.
The controller is manually developed using separate P, I, and D function blocks to better understand PID control behavior.

-Hardware
PLC: Siemens S7-1200
CPU: CPU 1214C DC/DC/Rly
I/O:
  Analog Input: Setpoint (SP), Process Variable (PV)
  Analog Output: Servo control signal

-Software
TIA Portal V16
Programming Language: Function Block Diagram (FBD)
PLC Software: STEP 7 Basic / STEP 7 Professional

-Control Logic
Read and scale SP and PV
Compute Error = SP − PV
Calculate control output using:
  P Controller (FC1)
  I Controller (FC2)
  D Controller (FC3)
Sum P, I, and D outputs to form the PID signal
Limit output and send to servo motor

-Conclusion
The system successfully demonstrates PLC-based PID control for a servo motor.
While P control provided the most stable response, PI and PID performance depended heavily on gain tuning.
This project highlights practical challenges in real-world PID implementation using PLCs.
