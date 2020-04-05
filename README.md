#### This sensor was abandoned because their is a 1-2 second delay in data output... The sensor output is also a saw-tooth and doesn't respond to quick starts and stops of airflow. An ongoing airflow sensor is here: [AFH55M12](https://github.com/hydronics2/COVID-19-Airflow-Sensor-AFH55M12) 

# Airflow - DegreeC Controls Sensor

## Project Description ([from Helpful Engineering](https://www.helpfulengineering.org/))
The intent here is to create a monitoring device, based on a mass airflow meter, that can be used when splitting a ventilator into two or more patients. This will allow staff to monitor individual patients while being controlled by one device in extreme situations where the number of ventilators are not enough to handle the number of patients. The readout should be visible locally on the device and there may need to be parameters input by staff to create a safe operating range and to possibly create alarms when the system is measuring an out of range parameter.


### [Project Requirements](https://docs.google.com/document/d/17Ps910A2vRwnM4EM6F-71GNG1XNa0PaeImd53F7428c/edit?usp=sharing)

This is a prototype using the [DegreeC controls F662-A air flow sensor](https://degree-controls-inc.myshopify.com/pages/f660-662)


![foo](https://github.com/hydronics2/COVID-19-Airflow-Sensor-DegreeC/blob/master/pics/f66x_sensor_pic.png)

Prototype board has an OLED screen and user interface rotary encoder and button.
![foo](https://github.com/hydronics2/COVID-19-Airflow-Sensor-DegreeC/blob/master/pics/board1.png)

Airflow sensor, humidity sensor and gauge pressure sensor is rear mounted.
![foo](https://github.com/hydronics2/COVID-19-Airflow-Sensor-DegreeC/blob/master/pics/board2.png)

![foo](https://github.com/hydronics2/COVID-19-Airflow-Sensor-DegreeC/blob/master/pics/pcb_on_tube.PNG)

A cavity in a tube exposes the sensors to the airstream.
![foo](https://github.com/hydronics2/COVID-19-Airflow-Sensor-DegreeC/blob/master/pics/pcb_on_tube2.PNG)



### Notes:
- Using a 1” diameter tube and normal inhale of 500mL gives an average air velocity of 0.328 m/s
	- 500 ml / (1.27 cm ^2 * pi) /3 sec/ 100.

### Bill of Materials
	- DegreeC Airflow sensor [f662-A](https://degree-controls-inc.myshopify.com/pages/f660-662)
	- gauge pressure sensor, MP3V5004G [NXP MP3V5004 Series](https://www.nxp.com/docs/en/data-sheet/MP3V5004G.pdf)
	- humidity sensor through-hole - H1H800, digikey 480-5706-1-ND
	- humidity sensor surface mount - SHTC3, digikey 1649-1100-1-ND
	- piezo buzzer, generic, 6.5mm pitch
	- transistor to drive piezo pn2222A
	- oled display, generic 1306 OLED, 128 x 64 pixels
	- Linear 3.3v regulator LDL1117S33R
	- Rotary Encoder and momentary switch, Bourns PEC12R-4220F-S0012-ND
	- generic 6mm user defined momentary tactile switch
	- generic 1206 smd LEDs for Power, Error, and TBD LED indicator
