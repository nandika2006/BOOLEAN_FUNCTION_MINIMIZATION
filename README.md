# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory** 

![image](https://github.com/user-attachments/assets/3efa61a9-e383-48b4-968b-c5039f11a9fa)


**Logic Diagram**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
```

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

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: RegisterNumber:24010030

```


**RTL realization**
Exp2_1 ![Screenshot (21)](https://github.com/user-attachments/assets/7a297d0e-1882-4a08-812a-10691b8805c2)


Exp2_2 ![Screenshot (23)](https://github.com/user-attachments/assets/4823f014-278c-4390-84e0-4e20733658c5)



**Timing Diagram**
Exp2_1 ![image](https://github.com/user-attachments/assets/0b763ba2-08ad-47bb-99ce-9fa4fda42d92)


Exp2_2 ![image](https://github.com/user-attachments/assets/0d70012e-db45-46ce-9cfb-bc80f6830b35)


**Result:**
Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

