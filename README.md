# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher 

**Software – Quartus prime** 

Cyclone V verilog program.

**Theory**

Boolean function minimization refers to the process of simplifying a Boolean
expression to its most efficient form. The goal is to reduce the number of logic gates,
variables, and terms needed to represent the function, which is important for hardware
design and optimization in digital circuits.

**Logic Diagram**
![Screenshot 2024-12-09 094305](https://github.com/user-attachments/assets/03834164-da83-4430-bcfe-2802210b33fe)


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

 module exp2(a,b,c,d,w,x,y,z,f1,f2);
 
 input a,b,c,d,w,x,y,z;
 
 output f1,f2;
 
 assign f1=((~b&~d)|(~a&b&d)|(a&b&~c));
 
 assign f2=((~y&z)|(x&y)|(w&y));
 
 endmodule


Developed by:Lathika Sree R RegisterNumber: 24009760


**RTL realization**
**Output:**
**RTL**


![Screenshot 2024-12-09 094305](https://github.com/user-attachments/assets/ef34efde-2f49-4c22-8d9b-a4e937f58f3b)


**Timing Diagram**


![Screenshot 2024-12-09 094358](https://github.com/user-attachments/assets/b48924ab-4929-4e34-85b1-ef9c5278f026)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

