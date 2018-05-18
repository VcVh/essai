# Helmet Impact Force Monitor adapted on Raspberry 2

The objective of this project is to measure the impact handled by a body during a fall and notice the user if medical attention is needed.

In fact, by impact we mean the force of the impact. And for that end, we will use an accelerometer to measure the G-force that is exerted on the body.
Studies have shown that G-force above 9G can be fatal and G-force between 4G and 6G can also be dangerous if sustained for a few seconds.

Our inpiration of this project comes from [this link](https://learn.sparkfun.com/tutorials/raspberry-pi-zero-helmet-impact-force-monitor?_ga=2.98552733.34402635.1521538802-1075053833.1521538802)

## Materials needed

* Raspberry Pi 2
	* with its power cable
	* a microSD card with NOOBS OS installed on it
* An accelerometer
	*We used a LISD2H accelerometer but we will explain how to adapt the code to yours
* An LED and its appropriate resistor
	*We used a red LED and a 1kohms resistor
* Some jumper wires

![alt text](https://github.com/VcVh/essai/blob/master/im.jpg "test")

## Configuration of your Raspberry

The easiest way to enable SSH and I2C on your device is by plugging a monitor, a keyboard and a mouse to it. Then power-up your card and open a terminal and type:
	* sudo apt-get update
	* sudo apt-get upgrade
	* sudo shutdown -r now

Then search for the configuration panel where you can enable both I2C and SSH.

Now you won't need the peripherals anymore but you will need to know the IP address of your card. You can find it using a software such as IP Tracker.
Once known, you are now able to control your Rapsberry Pi using Putty.

## Build the circuit

