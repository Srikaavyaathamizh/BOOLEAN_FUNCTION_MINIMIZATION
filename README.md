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

Developed by: SRIKAAVYAA T
RegisterNumber: 212223230214*/

```
module Boolean_min(A,B,C,D,W,X,Y,Z,F1,F2);

input A,B,C,D,W,X,Y,Z;

wire x1,x2,x3,x4,x5,x6,x7,x8,x9,x10;

output F1,F2;

assign x1=(~A)&(~B)&(~C)&(~D);

assign x2=(A)&(~C)&(~D);

assign x3=(~B)&(C)&(~D);

assign x4=(~A)&(B)&(C)&(D);

assign x5=(B)&(~C)&(D);

assign x6=(X)&(~Y)&(Z);

assign x7=(~X)&(~Y)&(Z);

assign x8=(~W)&(X)&(Y);

assign x9=(W)&(~X)&(Y);

assign x10=(W)&(X)&(Y);

assign F1=x1|x2|x3|x4|x5;

assign F2=x6|x7|x8|x9|x10;

endmodule
```

**RTL realization**

![Screenshot 2024-10-17 220345](https://github.com/user-attachments/assets/275e488b-baf4-4a79-bd9c-f72860b5ebac)
![Screenshot 2024-10-17 220352](https://github.com/user-attachments/assets/4b6dbd71-c0f1-45ad-b98f-6c3064214aee)


## LOGIC SYMBOL & Truthtable

![Screenshot 2024-10-17 220405](https://github.com/user-attachments/assets/e67af039-b3cc-446e-9ac5-6da07d477553)
![Screenshot 2024-10-17 220414](https://github.com/user-attachments/assets/dc46ee9c-f7dd-4daa-bcc8-84786c322922)

**Timing Diagram**

![Screenshot 2024-10-17 220428](https://github.com/user-attachments/assets/46d40db9-5441-4ddb-8e1b-8b5c1398434c)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

