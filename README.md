### ENCODER 8TO3 DATAFLOW Modelling

**AIM:**

To implement  Encoder 8 To 3 in Dataflow Modelling using verilog and validating their functionality using their functional tables

**SOFTWARE REQUIRED:** Quartus prime

**THEORY**

**Encoder 8 To 3**

The 8 to 3 line Encoder is also known as Octal to Binary Encoder. In 8 to 3 line encoder, there is a total of eight inputs, i.e., D0, D1, D2, D3, D4, D5, D6, and D7 and three outputs, i.e., A0, A1, and A2. In 8-input lines, one input-line is set to true at a time to get the respective binary code in the output side. Below are the block diagram and the truth table of the 8 to 3 line encoder.

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/0bc242c1-eb9e-4c47-afe5-30428470efc3)

Figure 01  Block Diagram of Encoder 8 * 3

**Truth Table**

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/35496b14-ae6e-4cd1-9abd-d6736b576575)

The logical expression of the term A0, A1, and A2 are as follows:

A0 = D1 + D3 + D5 + D7

A1 = D2 + D3 + D6 + D7

A2 = D4 + D5 + D6 + D7

Logical circuit of the above expressions is given below:

![image](https://github.com/naavaneetha/ENCODER8TO3DATAFLOW/assets/154305477/95acaee6-c873-4c75-89eb-ef09fb158053)

Figure 02  Encoder 8 * 3

**Procedure**

/* write all the steps invloved */

**PROGRAM**
```



# 8:3 ENCODER #


module enc(a,b,c,y0,y1,y2,y3,y4,y5,y6,y7);
input y0,y1,y2,y3,y4,y5,y6,y7;
output a,b,c;
assign a= ( y4 | y5 | y6 | y7);
assign b= ( y2 | y3 | y6 | y7);
assign c= ( y1 | y3 | y5 | y7);
endmodule
```

/* Program for Encoder 8 To 3 in Dataflow Modelling and verify its truth table in quartus using Verilog programming. 

Developed by:K.KARANKUMAR
RegisterNumber:25017410
*/

**RTL LOGIC FOR Encoder 8 To 3 in Dataflow Modelling**
<img width="586" height="384" alt="Screenshot 2025-12-14 181921" src="https://github.com/user-attachments/assets/7097a0c2-593b-4736-9a57-fee59c8e9168" />


**TIMING DIGRAMS FOR Encoder 8 To 3 in Dataflow Modelling**
<img width="580" height="240" alt="Screenshot 2025-12-14 181706" src="https://github.com/user-attachments/assets/b8c9d28c-36dd-497e-b023-4c18d5e3ddfc" />

**RESULTS**
Thus to implement Encoder 8 To 3 in Dataflow Modelling using verilog and validating their functionality using their functional tables is successfully verified



