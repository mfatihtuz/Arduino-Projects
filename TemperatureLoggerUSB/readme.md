Measuring temperature is a similar problem to measuring light intensity. Instead of an LDR, adevice called a thermistor is used. As the temperature increases, so does the resistance of the thermistor. 

When you buy a thermistor, it will have a statedresistance. In this case, the thermistor chosen is  33 KΩ.  This will be the resistance of the device at 25°C.

The formula for calculating the resistance at a particular temperature is given by: 

R=Ro^((-ß/(T+273)-ß/(To+273)) )

Rearranging this formula, we can get an expression for the temperature knowing the resistance. If we use a 33 KΩ fixed resistor, we can calculate the voltage at the analog input using the formula:
V=5*33K/(R+33K)
So,
R=((5*33K)/V)-33K
Since the analog value “a” is given by:
a=V*(1023/5)
then
V=a/205

and
R=(1025*33K/a)-33K

We can rearrange our formula to give us a temperature from the analog input, reading “a” as:

T=ß/(ln⁡(R/33)+(ß/298) )-273
and so finally we get:

T=ß/(ln⁡(((1025*33/a)-33)/33)+(ß/298) )-273

Phew, that’s a lot of math!

We will use this calculation in the next Project to create a temperature logger.
