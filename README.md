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
Create a new Quartus project: Launch Quartus Prime software and create a new project. Provide a name for your project and specify the location where you want to save it.

Design Entry: In the Quartus software, go to File > New > Project Wizard. Follow the wizard to specify the target device family, device, and any other relevant settings.
Compile the design: After designing your circuit or writing the Verilog/VHDL code, compile your design by clicking on Processing > Start Compilation.

Simulate your design: You can simulate your design using ModelSim, which is included with Quartus. This helps you verify that your design functions correctly.

Program your FPGA: Once your design is successfully compiled and simulated, you can program your FPGA using the Programmer tool in Quartus.

Test your design: After programming the FPGA, you can test your full encoder 8-to-3 to ensure it behaves as expected.

**PROGRAM**

/* Program for Encoder 8 To 3 in Dataflow Modelling and verify its truth table in quartus using Verilog programming. 

Developed by: Jabez S

RegisterNumber:212223040070
*/
**Encoder 8 * 3**
```
module ENCODER(D0,D1,D2,D3,A,B);
input A,B;
output D0,D1,D2,D3;
assign D0=((~A)&(~B));
assign D1=((~A)&B);
assign D2=(A&(~B));
assign D3=(A&B);
endmodule 
```

**RTL LOGIC FOR Encoder 8 To 3 in Dataflow Modelling**

![Screenshot 2024-04-04 133623](https://github.com/jabezs2005/ENCODER8TO3DATAFLOW/assets/147473463/15bd1b49-a9a3-4f25-b9bf-d2f9ddf16458)

**TIMING DIGRAMS FOR Encoder 8 To 3 in Dataflow Modelling**

![Screenshot 2024-04-04 143504](https://github.com/jabezs2005/ENCODER8TO3DATAFLOW/assets/147473463/d6243828-d703-4e25-bbd2-de922b688c37)

**RESULTS**

Successfully completed the encoder 



