# Simulation of Charge Pump using 28nm Technology

This repository presents the design of Charge pump. It is implemented using Synopsys Custom Compiler tool at 28nm technology node.
# Table Of Contents

 [1. Abstract](https://github.com/malihanaaz/Chargepump/edit/main/README.md#abstract)
 
 [2. Circuit Diagram of Charge Pump](https://github.com/malihanaaz/Chargepump/edit/main/README.md#cicruit-diagram-of-charge-pump)
 
 [3. Circuit Diagram of Non Overlapping Clock](https://github.com/malihanaaz/Chargepump/edit/main/README.md#circuit-diagram-of-non-overlapping-clock)
 
 [4. Implementation of Non Overlapping Clock](https://github.com/malihanaaz/Chargepump/edit/main/README.md#implementation-of-non-overlapping-clock)
 
   - [Inverter Schematic](https://github.com/malihanaaz/Chargepump/edit/main/README.md#inverter-schematic)
    
   - [Inverter Symbol](https://github.com/malihanaaz/Chargepump/edit/main/README.md#inverter-symbol)

   - [Inverter Testbench](https://github.com/malihanaaz/Chargepump/edit/main/README.md#inverter-testbench)
   
   - [Inverter Input & Output Waveforms](https://github.com/malihanaaz/Chargepump/edit/main/README.md#inverter-output-waveform)
   
   - [Nand Schematic](https://github.com/malihanaaz/Chargepump/edit/main/README.md#nand-schematic)
   
   - [Nand Symbol](https://github.com/malihanaaz/Chargepump/edit/main/README.md#nand-symbol)
   
   - [Nand Testbench](https://github.com/malihanaaz/Chargepump/edit/main/README.md#nand-testbench)
   
   - [Nand Input & Output Waveforms](https://github.com/malihanaaz/Chargepump/edit/main/README.md#nand-output-waveform)
   
   - [Non Overlapping Clock Schematic](https://github.com/malihanaaz/Chargepump/edit/main/README.md#non-overlapping-clock-schematic)
   
   - [Non Overlapping Clock Testbench](https://github.com/malihanaaz/Chargepump/edit/main/README.md#non-overlapping-clock-testbench)
   
   - [Non Overlapping Clock Input & Output Waveforms](https://github.com/malihanaaz/Chargepump/edit/main/README.md#non-overlapping-clock-output-waveform)
 
 [5. Implementation of 3- Stage Charge Pump](https://github.com/malihanaaz/Chargepump/edit/main/README.md#implementation-of-3-stage-charge-pump)
 
   - [Charge Pump Schematic](https://github.com/malihanaaz/Chargepump/edit/main/README.md#chargepump-schematic)
   
   - [Charge Pump Testbench](https://github.com/malihanaaz/Chargepump/edit/main/README.md#chargepump-testbench)
   
   - [Charge Pump Output Waveform](https://github.com/malihanaaz/Chargepump/edit/main/README.md#chargepump-output-waveform)

 [6. References](https://github.com/malihanaaz/Chargepump/edit/main/README.md#references)
 
 [7. Acknowledgement](https://github.com/malihanaaz/Chargepump/edit/main/README.md#acknowledgements)
 
 [8. About the Author](https://github.com/malihanaaz/Chargepump/edit/main/README.md#about-the-author)
   
# Abstract

This work presents an ultra-low Charge Pump for portable applications. A charge pump is a circuit that converts a power source to a greater or lower voltage based on the application. Charge pumps are commonly used in memory design since emerging memory technologies require a variety of power supplies.Charge pumps are basically inductor less 
Converters. The use of bulky inductors to increase the voltage is eliminated with the use of Charge pump circuits that work on only Capacitors and Switches. This saves the area of the circuit on Silicon. In this work, a 3 stage charge pump capable of operating at low voltages is presented.

# Cicruit Diagram of Charge Pump

A charge pump (CP) is an electrical circuit that converts the supply voltage VDD to a DC output voltage Vout that is several times greater than VDD. Capacitors and switches/diodes are the only components of CPs while the clock is supplied through non-overlapping clock. The circuit consists of two pumping clocks Φ1 and Φ2, which are non overlapping and have voltage amplitude as equal to supply voltage Vdd. MOS transistors are used instead of diodes. Through the coupling capacitors C1,C2–C4, the two clocks push the charge voltage upward through the transistors. A Non-overlapping Clock generator Circuit is used to generate two clocks which are equal in magnitude and are not in phase.

![3cp_circuit](https://user-images.githubusercontent.com/88283820/156145739-e8180c18-cd76-4908-bf24-49551c186921.png)

# Circuit Diagram of Non-Overlapping Clock

The Non- Overlapping Clock is implemented using Nand Gates and Inverters. Two Phases Phi1 and Phi2 which are non -overlapping are generated. Additonal inverters can be added to increase the delay.

![image](https://user-images.githubusercontent.com/88283820/156146350-1b8e18ae-b4a7-43bd-8bef-2a42b812e318.png)
# Implementation of Non-Overlapping Clock

This involves the implementation of Inverter and Nand Gates followed by the integration of these circuits to implement Non-Overlapping Circuit.

# Inverter Schematic
![inv_schem](https://user-images.githubusercontent.com/88283820/156008809-e2f2a45a-095c-4748-8f74-e784df71f367.PNG)

# Inverter Symbol
![inv_sym](https://user-images.githubusercontent.com/88283820/156008816-44ad703d-9610-4963-bb66-698a78e0d043.PNG)

# Inverter Testbench
![inv_tb](https://user-images.githubusercontent.com/88283820/156008819-aa8fabcc-1410-4ad1-8deb-716979a1c699.PNG)

# Inverter Input & Output Waveforms
![inv_out](https://user-images.githubusercontent.com/88283820/156008798-e5f90469-a64f-48b7-a512-c6b6984e613e.PNG)

# Nand Schematic
![nand_schem](https://user-images.githubusercontent.com/88283820/156008834-96b8409b-9b04-4998-84dd-b656ec50330a.PNG)

# Nand Symbol
![nand_sym](https://user-images.githubusercontent.com/88283820/156008840-e3cfd3a7-9772-4ffb-b47a-763e93de3a37.PNG)

# Nand Testbench
![nand_tb](https://user-images.githubusercontent.com/88283820/156008863-c3229943-4866-4a9f-950a-8ae8641b9849.PNG)

# Nand Input & Output Waveform
![nand_out](https://user-images.githubusercontent.com/88283820/156008825-aa4b610e-624d-4194-af4e-6842e87f97f9.PNG)

# Non Overlapping Clock Schematic
![noc_schem](https://user-images.githubusercontent.com/88283820/156008866-aef77d31-6f34-4ad3-8847-ee0e219a01e2.PNG)

# Non Overlapping Clock Testbench
![noc_tb](https://user-images.githubusercontent.com/88283820/156008875-3c982401-b527-4e53-9099-08e75cfe3059.PNG)

# Non Overlapping Clock Input & Output Waveform
![NOV](https://user-images.githubusercontent.com/88283820/156008639-1d4ece45-b857-4b1a-ac76-669f6ff8cb00.jpg)

# Implementation of 3-Stage Charge Pump:

The 3 Stage Charge pump is implemented with the help of diode connected MOSFETS, Capacitors and Non-Overlapping Clock. A large value Capacitor is used at the output to avoid ripples.

# Chargepump Schematic
![3stage_cp_schematic](https://user-images.githubusercontent.com/88283820/156171692-b7cb8cd2-5bb8-407b-be2c-66c479b4841f.PNG)

# Chargepump Testbench
![3stage_cp_testbench](https://user-images.githubusercontent.com/88283820/156173541-9a3380d0-36c6-48de-9ef0-9bc200d782d8.PNG)

# Chargepump Output Waveform
![3stage_cp_out](https://user-images.githubusercontent.com/88283820/156171721-d86a7f5a-980a-4c09-94a5-4e3e1f808390.PNG)

# References

[1] A. Kailuke, Pankaj Agrawal, R. Kshirsagar "Design and Implementation of low power Dickson Charge Pump in 0.18μm CMOS Process"  Published 2013 Engineering

[2]  Gaetano Palumbo, Domenico Pappalardo, “Charge Pump Circuits: An Overview on Design Strategies and Topologies”, Vol.10 ,Issue 1,15 March 2010, pp. 31-45.

[3]. G. Palumbo, D. Pappalardo, and M. Gaibotti, “Charge pump with adaptive stages for non-volatile memories,” IEE Proc. Circuits, Devices Syst., vol. 153, no. 2, pp. 136–142, Apr. 2006.


# Acknowledgements
     
  [1. Kunal Ghosh, Co- founder,VSD Corp. Pvt.Ltd](https://in.linkedin.com/in/kunal-ghosh-vlsisystemdesign-com-28084836)
  
  [2. Synopsys India](https://www.synopsys.com/)
  
  [3. IIT Hyderabad](https://iith.ac.in/)
  
  [4. Chinmaya Panda](https://ee.iith.ac.in/staff.html)
  
  [5. Sameer S Durgoji](https://in.linkedin.com/in/sameer-s-durgoji-340b26180)
     
# About the Author

Maliha Naaz, M.E (Digital Systems), Assistant Professor, Muffakham Jah College of Engineering & Technology & Part-Time Research Scholar at Osmania University, Hyderabad







