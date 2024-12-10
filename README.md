# FULL_ADDER_SUBTRACTOR

Implementation-of-Full-Adder-and-Full-subtractor-circuit

**AIM:**

To design a Full Adder and Full Subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime

**Full Adder and Full Subtractor**

**Full Adder**

Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin 

Carry = AB + ACin + BCin

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/0f30ba51-5ffb-4198-845f-18e054f675e7)

**Figure -1 FULL ADDER**

**Full Subtractor**

A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow.

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/02b24f51-ab51-4304-9ad6-7b81ffc1ead5)

Diff = A ⊕ B ⊕ Bin 

Borrow out = A'Bin + A'B + BBin

**Truthtable**
![ex 4 program](https://github.com/user-attachments/assets/a663e275-30db-4a09-8272-f6a2a297febf)
![ex 4 program 1](https://github.com/user-attachments/assets/a66d4eb4-4678-428a-b730-16f6dee673b3)

**Procedure**


Write the detailed procedure here

**Program:**
![ex 4 program 1](https://github.com/user-attachments/assets/4fe47de6-0e37-4366-ab34-e70f709a2690)
![ex 4 1](https://github.com/user-attachments/assets/c20531be-78a7-4817-8d80-c351e11b4e26)

/* Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming. Developed by: RegisterNumber:
*/

**RTL Schematic**
![ex 4 logic](https://github.com/user-attachments/assets/f88e0035-98f1-4d41-b515-deb32f1d980b)
![ex 4 logic 1](https://github.com/user-attachments/assets/5b26d76e-22b2-4b76-bd6f-85063b5052c4)

**Output Timing Waveform**
![ex 4 op](https://github.com/user-attachments/assets/ffd847ee-2e44-4692-9973-8229834d0a83)
![ex 4 op 1](https://github.com/user-attachments/assets/6740c112-dd16-478d-89c3-81daba4a3af1)

**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



