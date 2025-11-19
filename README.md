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
![WhatsApp Image 2025-11-19 at 10 31 17_db96595e](https://github.com/user-attachments/assets/3efe41ad-890b-4a70-be19-d6b1e1184900)


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

 Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:KOWSHIK RAM.S
RegisterNumber:25018630
```
module ex2(a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;

assign f1 = ((~b & ~d) | (~a & b & d) | (a & b & ~c));
assign f2 = ((~y & z) | (w & y) | (x & y));

endmodule
```

**RTL realization**
<img width="1920" height="1080" alt="Screenshot 2025-11-19 101440" src="https://github.com/user-attachments/assets/6a9f2ca0-8dc0-4ec4-a892-4e7aac41cf2b" />


**Output:**


**RTL**
<img width="1920" height="1080" alt="Screenshot 2025-11-19 102225" src="https://github.com/user-attachments/assets/8381a733-6948-45a7-9cc9-07af555d5349" />


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

