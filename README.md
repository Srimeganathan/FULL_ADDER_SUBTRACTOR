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
![170e3ab3-a7da-4759-ac4e-b3311f32dbd4](https://github.com/user-attachments/assets/ccf3ba0a-c4db-40cc-aa8a-ed18c626e05e)

**Procedure**


Write the detailed procedure here

**Program:**
Full Adder

module fulladder(sum, cout, a, b, cin); output sum;
output cout;
input a;
input b;
input cin;
wire w1,w2,w3;
assign w1=a^b;
assign w2=a&b;
assign w3=w1&cin;
assign sum=w1^cin;
assign cout=w2|w3;
endmodule 

Full Subtractor

module fullsub(df,bo,a,b,bin); 
output df;
output bo; 
input a; 
input b; 
input bin;
wire w1,w2,w3; 
assign w1=a^b; 
assign w2=(~a&b); 
assign w3=(~w1&bin); 
assign df=w1^bin; 
assign bo=w2|w3; 
endmodule
design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming. Developed by: RegisterNumber:
*/

**RTL Schematic**
![80103c29-ca04-42dc-bb5d-39daed6b00e7](https://github.com/user-attachments/assets/47eb5737-6676-442d-8686-ba88de91dd51)
![81712c0b-7809-47fc-9773-696d08137039](https://github.com/user-attachments/assets/ab79b461-ddcd-4144-ab1c-a79fc45d04ac)
![3c1e0a97-e532-4542-bb65-be0f8fa8d476](https://github.com/user-attachments/assets/d6afcd13-0ae9-4f7e-82dd-1f17b5a7a696)

**Output Timing 
![79f997fb-1fc5-4ba0-9235-b2ad8b4c59c8](https://github.com/user-attachments/assets/0214307a-b3d7-41e2-bdcf-d7db39e6c9df)Waveform**
![173c944a-65fb-4300-9f59-028843e135d3](https://github.com/user-attachments/assets/5c3aaf49-72f7-47fc-a72d-d50b3aed5a6e)

**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



