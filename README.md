Home Temperature Controller
===========================


This repository holds sources for a simple Home Temperature Controller I put together.



### Arduino

The **arduino** module contains source code and **libraries** that run controller of temperature for Arduion board.

The module is setup to send frequent updates of temperature reading via USB Serial port and receive a desired temperature setup via the same port.


### Temperature sensor reading and REST Server

The **temperature-sensor-and-rest** contains REST Server. 
It's responsibility is to:

* receive room temperature updates from Arduino board via USB Serial Port
* send desired temperature to Arduino board via USB Serial Port
* Store current and historical temperature reading in the simple File based DB
* TODO: send temperature updates to Arduino according to a pre-set schedule

### Controller web application designed for smartphones and tablets

The **ui/mobile-web-ui** contains code for a very simple User Interface, designed with Smartphones in mind. 
It's a set of static HTML files communicating with REST API, presenting current temperature reading and providing way of changing the desired setup.

TODO: Implementation of Scheduling UI to follow soon.


----




        License:
        I pretty much don't care what you do with the code, designs etc. Use it as you like.