# Stm32f103_HX711
Load sensor -HX711 -stm32f103c8 




Included dwt_delay library for microseconds delay.
Included CubeMX part

PA9 PIN -> SCK PIN 
PA10 PIN -> DATA PIN

-> With no load start than add some weight .
->Change your scale value untill get right value.
-> Datas are affecting from noise so much thats why be carefull about connections.

-> RED   -> A+
-> BLACK -> E-
-> WHITE -> E+
 
    BLACK SERIES 1K 
->(parallel)          -->  A-
    WHITE SERIES 1 K  
-> VCC  ->  +5V (Use External vcc)    
-> GND ->   GND 
-> SCK ->  PA9
-> DT  -> PA10