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

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 
```
Developed by: VIKASH S
RegisterNumber: 212225230302
module exp2(w,x,y,z,a,b,c,d,f1,f2);
input w,x,y,z,a,b,c,d;
output f1,f2;
assign f1=(~a&~b&~c&~d)|(a&~c&~d)|(~b&c&~d)|(~a&b&c&d)|(b&~c&d);
assign f2=(x&~y&z)|(~x&~y&z)|(~w&x&y)|(w&~x&y)|(w&x&y);
endmodule
```
truth table:
<img width="1012" height="556" alt="image" src="https://github.com/user-attachments/assets/b7eaa94f-4490-4401-b988-e43412fa8f99" />
<img width="1006" height="542" alt="image" src="https://github.com/user-attachments/assets/b5c8d804-f794-4289-9fd2-d1846a08732a" />
*/

**RTL realization**
<img width="958" height="498" alt="image" src="https://github.com/user-attachments/assets/221077df-e714-4207-8b0f-9fb82e4c6395" />

**Timing Diagram**
<img width="1906" height="963" alt="image" src="https://github.com/user-attachments/assets/2f7be414-8c6a-4af6-ba79-74b46d974e63" />

**Result:**
Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

