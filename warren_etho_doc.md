# WarrenLab_Ethocam Documentation



## Hardware Setup
* See the image detailing the outline of all of the wiring connections
	* However, with no Light Sensor and Relays

## Install WittyPi Software:
	`wget http://www.uugear.com/repo/WittyPi3/install.sh`
	`sudo sh install.sh`

## Package Installation:
* First install netifaces
	`sudo pip3 install netifaces`

* Perform circuit python installation on the raspberry pi (follow the steps in the below link)
	* (https://learn.adafruit.com/circuitpython-on-raspberrypi-linux/installing-circuitpython-on-raspberry-pi)
		* Makes base python python3 on the Pi
		* Run the blinkatest on the pi...

* Install the packages associated with the Temp/Humidity, Light Sensor, InkyPhat, GPS and WittyPi
	* For InkyPhat
		`sudo pip3 install inky`
	* Temp Humidity Sensor
		https://learn.adafruit.com/adafruit-si7021-temperature-plus-humidity-sensor/circuitpython-code
		`sudo pip3 install adafruit-circuitpython-si7021`
	* Light Sensor
		https://learn.adafruit.com/adafruit-tsl2591/python-circuitpython
		`pip install adafruit-circuitpython-tsl2591`
	* GPS:
		`pip install adafruit-circuitpython-gps`
	* WittyPi Python Package..:
		` git clone https://github.com/willdickson/py_wittypi_device.git `
		Now run the setup.py to initialize the w

* Install other Packages:
	* smbus2
		`pip3 install smbus2`

	* Paramiko:
		`pip install paramiko`
	* SCP:
		`pip install scp`
	* Font for the Display:
		`sudo pip3 install font-fredoka-one`


## Software:
* Go to github and clone the repo to the Pi. 
* the warren_control script can be used as a temporary method for controlling
the pi, and recording video, temperature, humidty and GPS.
* Make sure that everything has been converted to Python 3 from python2 using the package 2to3. Using 2to3 you can change everything within a directory. Additional manual changes may need to be made to finalize the conversion.
