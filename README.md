### Developed by:SRIRAM V
### Register Number: 212224050047
### Date : 06/05/2025
### EXPERIMENT 5: IMPLEMENTATION OF SYNCHRONOUS COUNTERS USING VERILOG HDL

### **AIM:**

To implement 4 bit synchronous up counter and validate functionality.

### **SOFTWARE REQUIRED:**

Quartus prime

### **THEORY**

### **4 bit synchronous UP Counter**

If we enable each J-K flip-flop to toggle based on whether or not all preceding flip-flop outputs (Q) are “high,” we can obtain the same counting sequence as the asynchronous circuit without the ripple effect, since each flip-flop in this circuit will be clocked at exactly the same time:

![image](https://github.com/naavaneetha/SYNCHRONOUS-UP-COUNTER/assets/154305477/d5db3fa0-e413-404c-b80e-b2f39d82e7e8)


![image](https://github.com/naavaneetha/SYNCHRONOUS-UP-COUNTER/assets/154305477/52cb61eb-d04b-442d-810c-31185a68410b)

Each flip-flop in this circuit will be clocked at exactly the same time.
The result is a four-bit synchronous “up” counter. Each of the higher-order flip-flops are made ready to toggle (both J and K inputs “high”) if the Q outputs of all previous flip-flops are “high.”
Otherwise, the J and K inputs for that flip-flop will both be “low,” placing it into the “latch” mode where it will maintain its present output state at the next clock pulse.
Since the first (LSB) flip-flop needs to toggle at every clock pulse, its J and K inputs are connected to Vcc or Vdd, where they will be “high” all the time.
The next flip-flop need only “recognize” that the first flip-flop’s Q output is high to be made ready to toggle, so no AND gate is needed.
However, the remaining flip-flops should be made ready to toggle only when all lower-order output bits are “high,” thus the need for AND gates.

### **Procedure**
### 1.Type the program in Quartus software.

### 2.Compile and run the program.

### 3.Generate the RTL schematic and save the logic diagram.

### 4.Create nodes for inputs and outputs to generate the timing diagram.

### 5.For different input combinations generate the timing diagram.

### **PROGRAM:**
![Screenshot 2025-05-06 103719](https://github.com/user-attachments/assets/184fc24c-bff0-4b54-9bdb-68d51deb9a67)



**RTL LOGIC UP COUNTER:**
![Screenshot 2025-05-06 103742](https://github.com/user-attachments/assets/06d558d7-6575-49c4-8f37-793928cb312a)



**TIMING DIAGRAM FOR IP COUNTER:**
![Screenshot 2025-05-06 104128](https://github.com/user-attachments/assets/aba40307-0087-4022-af7e-d496c4cf084d)

**TRUTH TABLE:**



![Screenshot 2025-05-06 104002](https://github.com/user-attachments/assets/5a4d60f8-9b52-4227-bd42-f583a450d2df)


**RESULTS:**
Thus the given 4 bit synchronous up counter are implimented using and validate functionality are verified using verilog programming.
