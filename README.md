# NAME:NITHISH S
# REFRENCE NUMBER: 23013509

# Experiment--02-Implementation-of-combinational-logic
Implementation of combinational logic gates
 
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
F2=xy’z+x’y’z+w’xy+wx’y+wxy
 
 
 
## Equipments Required:
## Hardware – PCs, Cyclone II , USB flasher
## Software – Quartus prime


##  Theory
A combinational circuit is a circuit in which the output depends on the present combination of inputs. Combinational circuits are made up of logic gates. The output of each logic gate is determined by its logic function. Combinational circuits can be made using various logic gates, such as AND gates, OR gates, and NOT gates.


##  Procedure
1. TYPE THE PROGRAM IN QUARTUS SOFTWARE.
2. COMPILE AND RUN THE PROGRAM.
3. GENERATE THE RTL SCHEMATIC AND SAVE THE LOGIC DIAGRAM.
4. CREATE NODES FOR  INPUTS AND OUTPUTS TO GENERATE THE TIMING DIAGRAM.
5. FOR DIFFERENT INPUT COMBINATIONS,GENERATE THE TIMING DIAGRAM

## Program:
```
module exp2de(A,B,C,D,F1);
input A,B,C,D;
output F1;
wire x1,x2,x3,x4,x5;
assign x1=(~A)&(~B)&(~C)&(~D);
assign x2=(A)&(~C)&(~D);
assign x3=(~B)&(C)&(~D);
assign x4=(~A)&(B)&(C)&(D);
assign x5=(B)&(~C)&(D);
assign F1=x1|x2|x3|x4|x5;
endmodule
```

##  RTL realization
![292724348-38b79db2-cb05-48b8-8030-dabf52481b61](https://github.com/Nithish23013509/Experiment--02-Implementation-of-combinational-logic-/assets/149038138/9a500e1b-57a5-4cc6-894c-9583f8aff61d)

## TRUTH TABLE
![292724406-60486c8e-7a97-4e65-9ce2-08b4b874ac2a](https://github.com/Nithish23013509/Experiment--02-Implementation-of-combinational-logic-/assets/149038138/8c9d2844-753f-4ee5-bcc4-b1e9220ffa6e)

##  Timing Diagram
![292724379-ea6e1572-26eb-4598-a11e-fdc0e0ceca65](https://github.com/Nithish23013509/Experiment--02-Implementation-of-combinational-logic-/assets/149038138/f307394c-c503-4401-bd6d-5b9b4014d776)

##  Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
