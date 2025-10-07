# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

**Logic Diagram**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
module funct1(a,b,c,d,f1);

input a,b,c,d;

output f1;

assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));

endmodule

module funct2(w,x,y,z,f2);

input w,x,y,z;

output f2;

assign f2=((~y & z)|( w & y )|(x & y));

endmodule


/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: RegisterNumber:*/


**RTL realization**
<img width="461" height="316" alt="Screenshot 2025-10-07 132143" src="https://github.com/user-attachments/assets/519c6d13-64a7-4e4e-979c-574ce64f8bb1" />
<img width="780" height="447" alt="Screenshot 2025-10-07 131028" src="https://github.com/user-attachments/assets/3ff7a161-a3c9-4861-99fa-4672511b1b48" />

**Timing Diagram**
<img width="1914" height="517" alt="Screenshot 2025-10-07 132117" src="https://github.com/user-attachments/assets/0580945a-7897-46d3-838b-6208f1ffd11f" />
<img width="1917" height="662" alt="Screenshot 2025-10-07 130959" src="https://github.com/user-attachments/assets/5ddd9cac-29d3-4a5e-9afa-948abee42b07" />


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

