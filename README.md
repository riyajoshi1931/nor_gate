# Implementation Of NOR GATE using CMOS
This repository presents the design & simulation of NOR GATE using 'Synopsis Custom Compiler Tool' using 28nm technology.
# Table Of Content
  1. [Abstract](#Abstract)
  2.  [Circuit_Details](#Circuit_Details)

  
  
  
  
  ### Abstract
  NOR GATE is a universal Logic gate. It can be used to build all other gates, also the complex circuits with higher number of transistor. A logic gate is physical design       that implements Boolean function. They are the building block of the high performance circuits. Its implementation is done using Synopsis Custom Design Tool. Here I am       using CMOS Technology because temperature stability, stronger anti-noise ability and lower power consumption.
  
  ### Circuit_Details
  For the design of any circuit with the CMOS technology; We need parallel or series connections of nMOS and pMOS with a nMOS source tied directly or indirectly to ground and   a pMOS source tied directly or indirectly to Vdd.
   Truth Table Of NOR GATE-
   ![Capture](https://user-images.githubusercontent.com/100508631/156124087-6f0713e1-2303-4140-9319-3fa667933560.PNG)
    Case-1 : A=0, B=0
        A=0: pMOS1 – ON; nMOS1 – OFF
        B=0: pMOS2 – ON; nMOS2 – OFF
        Path establishes from Vdd to Vout through the series connected ON pMOS transistors and Vout gets charged to Vdd level. No path from Vout to GND. Therefore, no             discharging and hence Vout will be High.
    Case-2 : A=0, B=1
        A=0: pMOS1 – ON; nMOS1 – OFF
        B=1: pMOS2 – OFF; nMOS2 – ON
        In this case path establishes from Vout to GND through nMOS2, but no path to Vdd. So, Vout would get discharged and will be at level Low.
    Case-3 : A=1, B=0
        A=1: pMOS1 – OFF; nMOS1 – ON
        B=0: pMOS2 – ON; nMOS2 – OFF
        The explanation is similar as case-2. Vout will be at level Low.
   Case-4 : A=1, B=1
        A=1: pMOS1 – OFF; nMOS1 – ON
        B=1: pMOS2 – OFF; nMOS2 – ON
        No path to Vdd. Path establishes from Vout to GND. So, Vout will be at level Low.


  
 
## Ref_ckt![ref_ckt](https://user-images.githubusercontent.com/100508631/156108235-38fd6d2f-4040-4bbe-89ca-4be23d39da20.png)
## Ref_Waveform![ref_waveform](https://user-images.githubusercontent.com/100508631/156119145-b424b992-1f3e-48ea-bcea-009e34241a10.png)
