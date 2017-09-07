# suraj-waghmare

project: creating tcp/ip client using pic18f67k22 and atwinc1500.

Problem: IRQN line of ATWINC1500 is always high, so the irq handler function is never called.

description:
IDE:- MPLAB X IDE v4.00.
COMPILER:- XC8 (V1.35)
CONTROLLER:- PIC18F67K22
WIFI MODULE:- ATWINC1500-MR210PB. firmware version (19.4.4)
using  MLA library for software.

We are using ready code for tcp/ip client from MLA library.
code path:-  \\mla\v2017_03_06\apps\tcpip\wifi_winc1500_demo\winc1500_pic18f87k22_ex8.X

Original software is written for PIC18F87K22, but we are using pic18f67k22, so we have done all necessary changes in code.

Original software is written for hardware external crystal, we are using internal clock to drive pic18f67k22. will this create any problem?

note:-
I can read and write data from atwinc1500 using “SPI communication”, also I can do UART communication to see results. But the problem is, “Interrupt event is not getting generated in atwinc1500 firmware”.

PROBLEM EXAMPLE:- ATWINC1500 gets connected to router, but it is not giving acknowledgement to pic18f67k22 that it is connected.

Suggest me solution.
