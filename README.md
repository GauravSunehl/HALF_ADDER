# HALF_ADDER
# AIM
To simulate and synthesis halfadder using xilinx ISE
# Appapratus required 
Xilinx 14.7 Spartan FPGA
# Procedure
step 1: start the Xilinx navigator, select and name the new project.
step 2: Select the device family,device package and speed.
step 3: Select new source in the new project and select verilog module as the source type.
step 4: type the file name and click next and finish button type the code save it.
step 5:  Select the behavioural simulation in the source windo and click the check syntax.
step 6: Click the simulation to simulate the program aand give the inputs and verify the outputs as per the truth table.
step 7: Select the implementation in the source window and select the required file in the process window 
Step 8: Select check syntax from the synthesized XST process double click in the floorplan area/IO/logic-post synthesize process in the user constraints process group.UCF (User constraint file) is obtained
step 9: In the designed object list window, enter the pin location for each pin in the location column select save from the file menu 
Step 10: Double click on the implement design and double click on the generate programming file to create a bitstream of the design.(.v) file is converted into.bitfile here.
step 11: Load the bitfile into the spartan 6 FPGA.
step 12: on the board by giving the required input the LEDs starts to glow light indicating the output

# Truth Table
![image](https://github.com/RESMIRNAIR/HALF_ADDER/assets/154305926/fe672c28-5c6a-4355-b70f-b40bce63880d)
# Circuit Diagram
![image](https://github.com/RESMIRNAIR/HALF_ADDER/assets/154305926/5f1a79a7-73c2-4b99-a40d-afa2a20c74ac)
# Sum = A XOR B
![image](https://github.com/RESMIRNAIR/HALF_ADDER/assets/154305926/020e1531-1c11-42e5-9f27-f09ba459984d)
# Carry = A AND B
![image](https://github.com/RESMIRNAIR/HALF_ADDER/assets/154305926/988ae131-0822-4d23-941b-eaafad349a72)

# Program
```
module half_adder(a,b,sum,carry);
input a,b;
output sum,carry;
xor g1(sum,a,b);
and g2(carry,a,b);
endmodule
```

# Output
![half adder 1](https://github.com/GauravSunehl/HALF_ADDER/assets/166976407/9464ecb7-cecb-45cb-97d4-52abd7a9a014)

# Result
Hence the halfadder output is verified.

