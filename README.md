ENCODER 8TO3 DATAFLOW Modelling AIM:

To implement Encoder 8 To 3 in Dataflow Modelling using verilog and validating their functionality using their functional tables

SOFTWARE REQUIRED: Quartus prime

THEORY

Encoder 8 To 3

The 8 to 3 line Encoder is also known as Octal to Binary Encoder. In 8 to 3 line encoder, there is a total of eight inputs, i.e., D0, D1, D2, D3, D4, D5, D6, and D7 and three outputs, i.e., A0, A1, and A2. In 8-input lines, one input-line is set to true at a time to get the respective binary code in the output side. Below are the block diagram and the truth table of the 8 to 3 line encoder.

The logical expression of the term A0, A1, and A2 are as follows:

A0 = D1 + D3 + D5 + D7

A1 = D2 + D3 + D6 + D7

A2 = D4 + D5 + D6 + D7

Procedure

1.Type the program in Quartus software.

2.Compile and run the program.

3.Generate the RTL schematic and save the logic diagram.

4.Create nodes for inputs and outputs to generate the timing diagram.

5.For different input combinations generate the timing diagram.

PROGRAM

module encodder(a0,a1,a2,d0,d1,d2,d3,d4,d5,d6,d7);
input d0,d1,d2,d3,d4,d5,d6,d7;
output a0,a1,a2;
assign a0 = d1|d3|d5|d7;
assign a1 =d2|d3|d6|d7;
assign a2 =d4|d5|d6|d7;
endmodule
Developed by SYED RAASHID HUSAIN M

RegisterNumber: 25009038

RTL LOGIC FOR Encoder 8 To 3 in Dataflow Modelling[rtl.pdf](https://github.com/user-attachments/files/24109468/rtl.pdf)


TIMING DIGRAMS FOR Encoder 8 To 3 in Dataflow Modelling [wave img.bmp](https://github.com/user-attachments/files/24109485/wave.img.bmp)


RESULTS

Thus the code is executed successfully.
