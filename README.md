# Heart rate-Monitor
 
This simple and inexpensive project is based around the MAX30100 sensor breakout board and utilizes a small 0.91" OLED display to report the heart rate and oxygenation level.
Both the devices used have an I2C two-wire interface and therefore keeps the wiring down to a minimum.

# The components required are:
 •	0.91” oled display
 •	Max30100 sensor breakout
 •	Dupont cable
 •	Arduino nano
 
 ![ARDUINO](https://images-wixmp-ed30a86b8c4ca887773594c2.wixmp.com/f/c82b5815-a4a2-4540-8dcd-d9fa8166dafa/da06lj6-9012becd-723d-4800-9c10-667ec0385708.jpg/v1/fill/w_1600,h_675,q_75,strp/minimal_arduino_wallpaper_2560x1080_by_dssdiego_da06lj6-fullview.jpg?token=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJzdWIiOiJ1cm46YXBwOiIsImlzcyI6InVybjphcHA6Iiwib2JqIjpbW3siaGVpZ2h0IjoiPD02NzUiLCJwYXRoIjoiXC9mXC9jODJiNTgxNS1hNGEyLTQ1NDAtOGRjZC1kOWZhODE2NmRhZmFcL2RhMDZsajYtOTAxMmJlY2QtNzIzZC00ODAwLTljMTAtNjY3ZWMwMzg1NzA4LmpwZyIsIndpZHRoIjoiPD0xNjAwIn1dXSwiYXVkIjpbInVybjpzZXJ2aWNlOmltYWdlLm9wZXJhdGlvbnMiXX0.zQD30vRSwuSArSk8Rqrw7GJQfBwAPl96VGi3JLEJ9Uc)
 
# Software requirements:
 •	Arduino IDE

# Hardware requirements:
 •	Soldering iron (generic)

# The wiring:
 Both the OLED display and the MAX30100 breakout board need 4 wires connected to the Arduino board:
 •	Ground
 •	VCC
 •	SDA
 •	SCL
 
**At start up, the display prompts the user to place their finger on the sensor. when it detects a heart beat updates the heart symbol on the display to show that and starts recording the readings.**

In my implementation I filter any measurement that is outside of a threshold and then calculate an average for both the heart rate and the SpO2 values and finally display that on the OLED.As long as the finger remains on the sensor and the sensor is detecting a hear beat, the display keeps showing the result. If the sensor does not detect a heart beat for 10 seconds, it restarts the process and prompts the user for another reading.



Thank you. :)
Cheers.
Happy Learning.










 


