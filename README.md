

 # ADS 1115 Example 


**Project Summary**

This project is written in RUST

It is running on a Raspberry PI 4

It is using 2, ADS1115 ADC chips

Make sure to add rppal = "0.17.0" to your Cargo.toml file. This is needed to use the I2C functionality. I strongly suggest reading the ADS1115 datasheet if you want interface and use the chip. It is very helpful at understading how to configure and use the chip. 


This project configures the ADS115 to run in continous sample mode (always returns ADC results) They are setup to saturate at 4.096V, singled ended ADC measurements, there are more configs than this.. just use the data sheet. This project has sevearl functions that request ACD channel samples, converts them reading to volts and prints the values. 

Useing 2 ADS115 chips, this lets us read 8 ADC value. 
