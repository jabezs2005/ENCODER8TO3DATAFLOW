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
Step1: Define the specifications and initialize the design. 

Step2: Declare the name of the entity and architecture by using VHDL source code. 

Step3: Write the source code in VERILOG. 

Step4: Check the syntax and debug the errors if found, obtain the synthesis report. 

Step5: Verify the output by simulating the source code. 

Step6: Write all possible combinations of input using the test bench. Step7: Obtain the place and route report

**PROGRAM
```
module enc(a,b,c,y0,y1,y2,y3,y4,y5,y6,y7);
input y0,y1,y2,y3,y4,y5,y6,y7;
output a,b,c;
assign a= ( y4 | y5 | y6 | y7);
assign b= ( y2 | y3 | y6 | y7);
assign c= ( y1 | y3 | y5 | y7);
endmodule
```

/* Program for Encoder 8 To 3 in Dataflow Modelling and verify its truth table in quartus using Verilog programming. 

Developed by: RegisterNumber:25018973
*/

**RTL LOGIC FOR Encoder 8 To 3 in Dataflow Modelling**
<img width="1920" height="1020" alt="2" src="https://github.com/user-attachments/assets/1285cecc-c564-4389-90dc-bd49b514d501" />

**TIMING DIGRAMS FOR Encoder 8 To 3 in Dataflow Modelling**
<img width="1920" height="1020" alt="3" src="https://github.com/user-attachments/assets/60f7be23-f853-46c5-bbf9-ee155dd981ec" />

**RESULTS**
Thus the encoder 8 to 3 data flow are designed and the truth tables is verified using quartus software



