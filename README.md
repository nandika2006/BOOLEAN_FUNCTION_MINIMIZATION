**NAME:** Nandika S


**REG-NO:** 24010030


## EXPERIMENT-2 BOOLEAN FUNCTION MINIMIZATION


**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory** 

Implementing Boolean functions in Verilog HDL (Hardware Description Language)
involves translating the simplified Boolean expressions into Verilog code to describe the
behavior of digital circuits. The basic building blocks in Verilog is module. The module
represent a combinationa circuit. Use logical operators (&, , ~, ^) to implement Boolean
functions directly. Use built-in gate primitives for basic functions: Use University
program VWF to verify the functionality of your Verilog modules. Create waveform and
check outputs against expected results

![image](https://github.com/user-attachments/assets/3efa61a9-e383-48b4-968b-c5039f11a9fa)


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

module Exp2_1(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b&~d)|(~a&b&d)|(a&b&~c));
endmodule

module Exp2_2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y&z)|(x&y)|(w&y));
endmodule

**Truth Table**

![image](https://github.com/user-attachments/assets/1c5f3fe9-ca4b-42e1-b616-23f746e1def1)


**RTL realization**
![image](https://github.com/user-attachments/assets/114a75a4-d17e-4511-8457-7bf9d9861f0a)



**Timing Diagram**
Exp2_1 ![image](https://github.com/user-attachments/assets/0b763ba2-08ad-47bb-99ce-9fa4fda42d92)


Exp2_2 ![image](https://github.com/user-attachments/assets/0d70012e-db45-46ce-9cfb-bc80f6830b35)


**Result:**
Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

