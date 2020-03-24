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
