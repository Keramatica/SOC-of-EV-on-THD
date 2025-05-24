# SOC-of-EV-on-THD
State of Charge Influence on the Harmonic Distortion From Electric Vehicle Charging
This simulation analyzes how EV battery state of charge (SOC) and charging algorithms affect current harmonic distortion (THD). Real data was collected from EV charging stations in Colombia and Germany using five EV models.
Key findings:
•	Different charging algorithms (CC, MCC, CCCV) were tested.
•	BMW i3, the only car using 3-phase AC, showed distinct harmonic behavior.
•	A MATLAB/Simulink model simulated CCCV algorithm using a Li-ion battery and AC-DC + buck converter with a 40 kHz PWM.
Simulation results:
•	Current THD increases as battery voltage reaches the CCCV transition point.
•	Using the paper’s filter values (e.g., 2000 µF capacitor) led to higher-than-expected source current.
•	Adjusting C1 from 2000 µF to 500 µF aligned voltage and current more closely with expected values, but did not significantly reduce THD.
•	Final THD values did not fully match the experimental results, suggesting further tuning of filter parameters is needed.

