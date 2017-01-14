# Grupp4 - A sound alerted surveillance camera


##Directory tree
.
+-- Code		#Contains all source- & test codes for the project
	|
	+-- Arduino Library		#Libraries for Arduino IDE needed to compile source code 
  	|	|
  	|	+-- ESP8266Scheduler		#Scheduler for tasks on Arduino IDE for Feather HUZZAH ESP8266
	+-- HUZZAH		#Source code for Feather HUZZAH ESP8266
		|
  		+-- Feather HUZZAH Serial Drivers #Mac, Windows, Linux or Android serial drivers for Feather HUZZAH
  		+-- Hardware Test Codes #Projects for testing hardware


##Setting up Feather HUZZAH w/ ESP8266

###Install serial drivers
There are serial drivers compatible with Mac, Windows, Linux and Android
Install serial drivers located in "Code->HUZZAH->Feather HUZZAH Serial Drivers" or download from:
https://www.silabs.com/products/mcu/Pages/USBtoUARTBridgeVCPDrivers.aspx

###Connecting with serial(for LUA programming)
Connect Feather HUZZAH through USB-cable to your computer.
Use a serial console app like CoolTerm (Mac) or Putty (Windows) or screen (linux).
Connect to the serial port using the console app with 9600bps
Press the RESET button on the HUZZAH to print out the welcome message on the serial console

###Connecting & programming with Arduino IDE
Open Arduino IDE Preferences
Enter this into Additional Boards Manager URLs: http://arduino.esp8266.com/stable/package_esp8266com_index.json
Press OK
Go to Tools -> Board -> Board Manager
Install "esp8266 by ESP8266 Community"
Restart Arduino IDE
Select "Adafruit HUZZAH ESP8266" in Tools -> Board
Select 80MHZ in CPU Frequency
Select 4M (3M SPIFFS) in Flash Size
Select 115200 baud rate
Select Serial port
Ready to upload code!
Recommended to try a test code in "Code->HUZZAH->Hardware Test Codes" to verify that everything is working