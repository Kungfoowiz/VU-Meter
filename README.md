# VU-Meter
Volume Unit (VU) Meter micro circuit project - modulates AC speaker output to DC VU Meter.

## Circuit Diagram
This diagram covers the same circuit for both speakers, left and right, they are identical.

AMP SPEAKER (+)
   |
   |    [ R1 ]        [ VR1 ]          [ D1 ]
   o---/\/\/\/\--------(5k)----------->|--------o  METER (+)
        220–470Ω      Trimpot      1N60 / BAT42 |
                                                |
                                                |   [ C1 ]
                                              ----- 47–100uF
                                              ----- (Smooth)
                                                |
AMP SPEAKER (–) ---------------------------------o  METER (–)

