This is a modification of the ../blinky example that made a couple  
optimizations to enabled LED dimming using Pulse Width Modulation  
of the LED signals. PWM is accomplised by using a subset of bits in  
the counter to derive a pulse on off signal. Similarly, instead of  
decimating the clock counter it just grabs the high order counter bits  
for the LED interval.  
  
button 0 is used to enable and disable LED lighting and to reset the count  
button 1 is used disable the PWM and illuminate at full brightness.  


Note: this is tested on v1.3 HW before the new LED resistors change.  
This means that the current dimming may be too dull on the most recent  
spin of v1.3. You can select more or fewer bits on line 41 or a different  
mask to adjust the pulse widths.  
