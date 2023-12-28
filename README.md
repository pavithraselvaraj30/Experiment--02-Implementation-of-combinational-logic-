# Experiment--02-Implementation-of-combinational-logic
Implementation of combinational logic gates
 
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
F2=xy’z+x’y’z+w’xy+wx’y+wxy
 
 
 
## Equipments Required:
## Hardware – PCs, Cyclone II , USB flasher
## Software – Quartus prime


## Theory
 A combinational circuit is a circuit in which the output depends on the present combination of inputs. Combinational circuits
are made up of logic gates. The output of each logic gate is determined by its logic function. Combinational circuits can be
made using various logic gates, such as AND gates, OR gates, and NOT gates.

## Logic Diagram
## Procedure
1.Type the program in Quartus software.
 2.Compile and run the program.
 3.Generate the RTL schematic and save the logic diagram.
 4.Create the nodes for inputs and outputs to generate the timing diagram.
 5.For the different input combination,generate the timing diagram.
## Program:
```

/*
Program to implement the given logic function and to verify its operations in quartus using Verilog programming.
Developed by:pavithra.s 
RegisterNumber: 212223230147 
module ex_02(a,b,c,d,f1);
input a,b,c,d;
output f1;
wire x1,x2,x3,x4,x5;
assign x1=(~a)&(~b)&(~c)&(~d);
assign x2=(a)&(~c)&(~d);
assign x3=(~b)&(c)&(~d);
assign x4=(~a)&(b)&(c)&(d);
assign x5=(b)&(~c)&(d);
assign f1=x1|x2|x3|x4|x5;
endmodule
*/
```
## RTL realization
![WhatsApp Image 2023-12-28 at 20 18 14_e447e856](https://github.com/pavithraselvaraj30/Experiment--02-Implementation-of-combinational-logic-/assets/149366880/e4b4a055-d21b-485e-ac28-4963b2971305)
## Truth Table:

![WhatsApp Image 2023-12-28 at 20 19 11_05beba0d](https://github.com/pavithraselvaraj30/Experiment--02-Implementation-of-combinational-logic-/assets/149366880/c72e4378-24b2-43d2-8e2c-102ec9c0636c)

## Timing Diagram:
![WhatsApp Image 2023-12-28 at 20 19 39_5b699d5e](https://github.com/pavithraselvaraj30/Experiment--02-Implementation-of-combinational-logic-/assets/149366880/24947d76-a2be-4267-8750-6a3b4304ae61)

## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
