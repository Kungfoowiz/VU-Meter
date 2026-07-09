# VU-Meter  
Volume Unit (VU) Meter micro circuit project - modulates from an AC speaker output to a DC VU Meter.  
  
## Circuit Diagram
This diagram shows the circuit and can be used for both left and right speakers.

<img width="521" height="322" alt="image" src="https://github.com/user-attachments/assets/3325bed3-bec1-4e22-82a5-b87c1ab5841d" />

## Signal Path Explanation

**From Amp Speaker (+):** The audio signal leaves the amplifier's positive speaker terminal.  
  
**Through Variable Resister (VR1):** The signal first passes through the 1KΩ variable resistor (VR1), controlling strength of signal into the VU Meter. Increased resistance gives decreased sensitivity, weaker signal, and reduced VU meter movemement. 
  
**Through Diode (D1):** After VR1, the signal goes into the 1N60 (BAT42) diode (D1), which rectifies the alternating current (AC) audio signal into pulses of direct current (DC). 
  
**Into VU Meter (+):** The rectified DC signal from D1 then enters the positive (+) terminal of the VU Meter, causing the needle needle to move based on the average of the DC pulses.  
  
**Capacitor (C1) across the VU Meter (-) and (+) termains:** The 47 microfarad (µF) capacitor is connected between VU Meter (+) and VU Meter (–) terminals, smoothing the rectified DC signal and turning sharp pulses into smooth pulses, by averaging the voltage and preventing needle jitter.  
  
**Back to Amp Speaker (–):** Finally, the return DC signal path from VU Meter (–) terminal goes back to the amplifier’s negative speaker terminal, completing the circuit.  
