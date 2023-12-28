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
![WhatsApp Image 2023-12-28 at 20 05 17_7fb52325](https://github.com/pavithraselvaraj30/Experiment--02-Implementation-of-combinational-logic-/assets/149366880/40798366-72c8-4811-82bd-4cc90686a6d6)



## Truth Table:

![WhatsApp Image 2023-12-28 at 20 05 12_149aed52](https://github.com/pavithraselvaraj30/Experiment--02-Implementation-of-combinational-logic-/assets/149366880/96f0fdfb-5efc-480f-8007-c78c87f523eb)

## Timing Diagram:
![WhatsApp Image 2023-12-28 at 20 05 12_8bc0048c](https://github.com/pavithraselvaraj30/Experiment--02-Implementation-of-combinational-logic-/assets/149366880/d5d7d12e-6c95-4c60-817a-d720c0e62ad4)

## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
