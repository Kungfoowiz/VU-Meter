# VU-Meter  
Volume Unit (VU) Meter micro circuit project - modulates AC speaker output to DC VU Meter.  
  
#### Circuit Diagram
This diagram covers the same circuit for both speakers, left and right, they are identical.  

<img width="552" height="216" alt="image" src="https://github.com/user-attachments/assets/b1344f87-e6d0-4ce3-8c80-fe140dcbc38d" />

#### Signal Path Explanation

**From AMP SPEAKER (+):** The audio signal leaves the amplifier's positive speaker terminal.  
**Through Variable Resister (VR1):** The signal first passes through the 1,000 Ω potentiometer. This controls how strong the signal is that reaches the meter.  Turning it up increases meter movement (higher sensitivity), turning it down reduces movement.  
  
**Through Diode (D1):** After VR1, the signal goes into the 1N60/BAT42 diode. The diode rectifies the AC audio into a pulsed DC signal so the meter can respond in one direction instead of swinging back and forth.  
  
**Into VU METER (+):** The rectified signal then enters the positive terminal of the VU meter, causing the needle to move according to the average level of the audio.  
**Capacitor (C1) across the meter:** The capacitor is connected between METER (+) and METER (–). It smooths the rectified signal, turning sharp pulses into a more averaged voltage so the needle moves smoothly instead of jittering.  
**Back to AMP SPEAKER (–):** Finally, the return path from METER (–) goes back to the amplifier’s negative speaker terminal, completing the circuit.  


  
