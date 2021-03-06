# Heart rate-Monitor
 
This simple and inexpensive project is based around the MAX30100 sensor breakout board and utilizes a small 0.91" OLED display to report the heart rate and oxygenation level.
Both the devices used have an I2C two-wire interface and therefore keeps the wiring down to a minimum.

# The components required are:
 •	0.91” oled display
 •	Max30100 sensor breakout
 •	Dupont cable
 •	Arduino nano
 
  ![LED](https://www.electronicscomp.com/image/cache/catalog/0.91-inch-oled-display-module-800x800.jpg)
  
  ![MAX30100](https://i0.wp.com/zbotic.in/wp-content/uploads/2021/02/AI0240.jpg)

# Software requirements:
 •	Arduino IDE
 
  ![ARDUINO](https://www.vernier.com/wp-content/uploads/2020/05/Arduino-Loop-logo-768x492.png)

# Hardware requirements:
 •	Soldering iron (generic)

# The wiring:
 Both the OLED display and the MAX30100 breakout board need 4 wires connected to the Arduino board:
 •	Ground
 •	VCC
 •	SDA
 •	SCL
 
  ![Picture1](https://user-images.githubusercontent.com/32995285/110212283-ab700d00-7ec0-11eb-836d-e29d6e8ab9d3.png)

 
**At start up, the display prompts the user to place their finger on the sensor. when it detects a heart beat updates the heart symbol on the display to show that and starts recording the readings.**

In my implementation I filter any measurement that is outside of a threshold and then calculate an average for both the heart rate and the SpO2 values and finally display that on the OLED.As long as the finger remains on the sensor and the sensor is detecting a hear beat, the display keeps showing the result. If the sensor does not detect a heart beat for 10 seconds, it restarts the process and prompts the user for another reading.



Thank you. :)
Cheers.
Happy Learning.










 


