# Full-Adder-Using-CMOS-Mirror-Logic
This repository presents the Design Of 1-Bit Full Adder Using CMOS Mirror Logic implemented using Synopsis Custom Compiler on 28nm CMOS Technology.
# Abstract
This paper presents a 1-bit full adder cell designed by using the CMOS mirror technique. The full adder circuit is one of the most widely used building blocks in all arithmetic and digital data processing systems. This circuit accepts two 1-bit inputs and produces two 1-bit outputs i.e. sum and carry. We use the property of inversion and self-duality to design this circuit. Because nowadays we have to deal with huge bits of data, we can switch to more advanced adder architectures like  RIPPLECARRY, CARRYSKIP, CARRYSELECT, CARRYLOOKAHEAD, etc. The major drawback of the CMOS mirror circuit is that it consumes more power and occupies more area due to the greater number of transistors used.
# Tools Used
*Synopsys Custom Compiler:  The Synopsys Custom Compiler™ design environment is a modern solution for full-custom analog, custom digital, and mixed-signal IC design. As the heart of the Synopsys Custom Design Platform, Custom Compiler provides design entry, simulation management and analysis, and custom layout editing features. This tool was used to design the circuit on a transistor level.


# Circuit Details
Transistor level implementation of full adder using CMOS mirror logic uses transistors which has nmos and  pmos. By using CMOS mirror design we can save an area of 12 transistors as compared to the conventional CMOS approach. If a function obeys both inversion and self-duality properties then we can mirror the nmos stack to pmos i.e. pull-up stack is symmetrical to pull-down, unlike the opposite to pull-down stack in conventional CMOS. By this approach, we can reduce pmos stack size and can have equal rise and fall delays. Instead of realizing two functions independently, we will use cout signal to generate sum signal. The full adder circuit presented in this paper can be further used as a building block to generate an N-bit adder, which accepts two n-bit inputs and produces n-bit sum. One such adder architecture is known as ripple carry adder where these full adder blocks are cascaded one after the other. Each full adder in this architecture produces a 1-bit sum and passes the carry to the subsequent full adder. In this way carry ripples through each of the full adder stages. Speed of this carry rippling through each stage define the speed of the adder. Nowadays there are some advancedstatic CMOS techniques like CPL, TG, GDI, etc., to design a high speed and low power consumption full adder but tuning the circuit alone is not the feasible solution as we have to deal with huge bits of data at a time. In this case,optimizing the architecture of the adder circuit can come in handy.
# Reference Circuit
![Refernce circuit of 1-bit full adder using CMOS mirror logic](https://user-images.githubusercontent.com/98546502/155892419-00f1960a-94c9-419e-84a8-6752c2f3b6b9.png)
# Reference waveform
![1bit full adder sample wave form](https://user-images.githubusercontent.com/98546502/155892517-8a195f0b-c824-427f-a349-d70b237dad72.png)
#Truth table
![1bit full adder truth table](https://user-images.githubusercontent.com/98546502/155892607-84e23f36-1cc3-4a27-bfd4-f53f23df1e03.jpg)
# 
