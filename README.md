# VU-Meter  
Volume Unit (VU) Meter micro circuit project - modulates from an AC speaker output to a DC VU Meter.  
  
https://github.com/user-attachments/assets/a8d7fb70-e60c-4418-8006-6863ea896f44  

  
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

  
<img width="504" alt="941f92b7-8035-45ff-8b32-d8be38886f5b" src="https://github.com/user-attachments/assets/ca8d0cf4-85ca-4f9a-936f-2dc0f43dc122" />  

  
<img width="504" alt="dc6a33de-d280-4362-becf-5c78c7ca062e" src="https://github.com/user-attachments/assets/b64ee38f-698a-4116-8a9c-1f2687d84292" />  

  
<img width="504" alt="0e0de804-92ea-499d-882e-a3b39d6013d6" src="https://github.com/user-attachments/assets/e62d0325-8ac3-4586-a60d-9f4238fdaa0b" />  

  
<img width="504" alt="87c017db-489f-41a8-90d1-57d1e8d47be7" src="https://github.com/user-attachments/assets/1773a99c-6601-420f-a962-356c55de71f2" />  

  
<img width="504" alt="4f4e3594-ce92-4bbc-9b8c-68d7b64e6e25" src="https://github.com/user-attachments/assets/b08a7167-d1b8-4f01-bd2b-286d0d852faf" />  


    
