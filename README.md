# Linear-Feedback-Shift-Register-using-LTSpice
This git contains all the files and instructions required to create a LFSR using D-Flip Flops in LTSpice.

**Linear Feedback Shift Register**

A LFSR is a sequential shift register with a feedback path that is used to generate a sequence of pseudo-random binary values. It consists a series of D flip-flops 
connected in a chain. A feedback path is via the MSB of the generated sequence, through a network of XOR gates.

**Components used** (LTSPICE inbuilt library):
1. **DFlop**: Component > Digital > DFlop
2. **xor**: Component > Digital > xor

**Seed Value Generator:**

A separate seed value generator has been implemented to generate a one bit output, that would act as a **"Set"** value for the D-Flip Flop.

![image](https://github.com/dhrupad-u/Linear-Feedback-Shift-Register-using-LTSpice/assets/42469685/e3a6124e-3344-48f8-9dd6-6f33af5244eb)

**A 4-bit LFSR**

Here is the implementation of a 4-bit LFSR:

![image](https://github.com/dhrupad-u/Linear-Feedback-Shift-Register-using-LTSpice/assets/42469685/fa4c103f-eec9-4791-87f7-640242f9c688)

Simulation of the 4-bit LFSR:

![image](https://github.com/dhrupad-u/Linear-Feedback-Shift-Register-using-LTSpice/assets/42469685/1841c772-d1cc-4bad-a23e-3b3b3b9cfd77)

Once this is implemented, we can convert it into a symbol and cascade it further to create a 2^n bit LFSR.

Cascading of 4 * 4-bit LFSR's:

![image](https://github.com/dhrupad-u/Linear-Feedback-Shift-Register-using-LTSpice/assets/42469685/027ebccb-78dd-4c70-9aa0-13b5e961d4e9)

Simulation of the 16-bit LFSR:

![image](https://github.com/dhrupad-u/Linear-Feedback-Shift-Register-using-LTSpice/assets/42469685/72b19ca4-a1b8-4e14-a786-2cf59629f09c)

This can be cascaded further as per requirement. 

Make sure to initialize each inbuilt D-Flip Flop as follows:

![image](https://github.com/dhrupad-u/Linear-Feedback-Shift-Register-using-LTSpice/assets/42469685/2420f395-7b80-4eaa-8625-7e2eae6a9c73)

**Files included**
1. 4-bit LFSR schematic (.asc file)
2. 4-bit LFSR symbol (.asy file)
3. 16-bit LFSR schematic (.asc file)


