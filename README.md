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
~~~
/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming.

Developed by: HARRISH VENKAT V
Register Number:212223240049

module Boolean_min(a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
wire adash,bdash,cdash,ddash,ydash,p,q,r,s,t,u;
not(adash,a);
not(bdash,b);
not(cdash,c);
not(ddash,d);
not(ydash,y);
and(p,bdash,ddash);
and(q,adash,b,d);
and(r,a,b,cdash);
or(f1,p,q,r);
and g1(s,ydash,z);
and g2(t,x,y);
and g3(u,w,z);
or g4(f2,s,t,u);
endmodule
~~~

## RTL realization output

![image](https://github.com/HarrishVenkat/BOOLEAN_FUNCTION_MINIMIZATION/assets/144979588/a7f3675f-40d4-416d-95f9-f83d54f83c27)

## Truth table
![image](https://github.com/HarrishVenkat/BOOLEAN_FUNCTION_MINIMIZATION/assets/144979588/09f2ae55-3fe9-4fc6-b1b3-321c9ea3731c)

## Timing Diagram

![image](https://github.com/HarrishVenkat/BOOLEAN_FUNCTION_MINIMIZATION/assets/144979588/5831b659-3050-45a5-8db4-ab031948a2c4)

## Result:

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

