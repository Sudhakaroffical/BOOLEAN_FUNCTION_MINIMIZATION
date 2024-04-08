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
```
Developed by: SUDHAKAR K

RegisterNumber:212222240107

*/
```

**RTL realization**

![DE 2A](https://github.com/Rama-Lekshmi/BOOLEAN_FUNCTION_MINIMIZATION/assets/118541549/edc9e43f-2899-43eb-8a8e-2e331fda6c39)

**Output:**


![DE 2B](https://github.com/Rama-Lekshmi/BOOLEAN_FUNCTION_MINIMIZATION/assets/118541549/228dd854-2beb-4e42-b0bc-0c3848edc457)


## Logic symbol & Truthtable:

![DE 2C](https://github.com/Rama-Lekshmi/BOOLEAN_FUNCTION_MINIMIZATION/assets/118541549/1320c49e-13f6-45f6-a28d-63a4c5fde8cd)


![DE 2D](https://github.com/Rama-Lekshmi/BOOLEAN_FUNCTION_MINIMIZATION/assets/118541549/2b76ba1f-67ec-4969-b9c6-8f0b975f551f)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

