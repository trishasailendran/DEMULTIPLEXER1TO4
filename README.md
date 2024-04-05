# DEMULTIPLEXER1TO4
# Aim:
To simulate and synthesis DEMULTIPLEXER 1 TO 4 using Vivado software.
# Software Required:
Vivado 2023.1 software.
# Procedure 
STEP:1 Start the Xilinx navigator, Select and Name the New project.

STEP:2 Select the device family, device, package and speed.

STEP:3 Select new source in the New Project and select Verilog Module as the Source type.

STEP:4 Type the File Name and Click Next and then finish button. Type the code and save it.

STEP:5 Select the Behavioral Simulation in the Source Window and click the check syntax.

STEP:6 Click the simulation to simulate the program and give the inputs and verify the outputs as per the truth table.

STEP:7 Select the Implementation in the Sources Window and select the required file in the Processes Window.

STEP:8 Select Check Syntax from the Synthesize XST Process. Double Click in the Floorplan Area/IO/Logic-Post Synthesis process in the User Constraints process group. UCF(User constraint File) is obtained.

STEP:9 In the Design Object List Window, enter the pin location for each pin in the Loc column Select save from the File menu.

STEP:10 Double click on the Implement Design and double click on the Generate Programming File to create a bitstream of the design.(.v) file is converted into .bit file here.

STEP:11 Load the Bit file into the SPARTAN 6 FPGA

STEP:12 On the board, by giving required input, the LEDs starts to glow light, indicating the output.

![image](https://github.com/RESMIRNAIR/DEMULTIPLEXER1TO4/assets/154305926/b6d81e6c-81ec-4f91-ae42-832a68f8facc)
# Truth Table
![image](https://github.com/RESMIRNAIR/DEMULTIPLEXER1TO4/assets/154305926/bb0a83c7-b4f3-463b-b422-f2ff65b1a0ee)
# Circuit Diagram
![image](https://github.com/RESMIRNAIR/DEMULTIPLEXER1TO4/assets/154305926/dcd56444-97dd-454b-bddf-c7472c4af1de)
![image](https://github.com/RESMIRNAIR/DEMULTIPLEXER1TO4/assets/154305926/03fbbbdf-8ae3-4653-8047-7d4cbf555ccb)
![image](https://github.com/RESMIRNAIR/DEMULTIPLEXER1TO4/assets/154305926/f48cc07d-c76f-4d1c-8907-11e99711b751)
![image](https://github.com/RESMIRNAIR/DEMULTIPLEXER1TO4/assets/154305926/a3075cf9-55ba-4478-b20c-c7128badef04)
![image](https://github.com/RESMIRNAIR/DEMULTIPLEXER1TO4/assets/154305926/e07386db-69b3-4a5f-945f-b38929b801ea)
# Program
 ```
Developed by: Trisha S
Register number: 212222060280
```
```
module demux(y0,y1,y2,y3,s1,s0,I);
 input I,s0,s1;
 output y0,y1,y2,y3;
     assign s1n = ~ s1;
     assign s0n = ~ s0;
     assign y0 = I & s0n & s1n;
     assign y1 = I & s0 & s1n;
     assign y2 = I & s0n & s1;
     assign y3 = I & s0 & s1;
 endmodule
```
# Output
<img width="768" alt="318172064-5ae7b88b-d5e1-4a3c-93fe-dd64e73574cd" src="https://github.com/trishasailendran/DEMULTIPLEXER1TO4/assets/87655678/b85cee91-2655-4673-aa17-e3dbb0da80c4">

# Result
Thus the simulate and synthesis of DEMULTIPLEXER 1 TO 4 is verified successfully by using Vivado software.

