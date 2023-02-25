# Hardware Proposal

With a big goal in mind the team has been tasked with separate functions within the building process of the product. Each team ember has been given a complex set of parts called subsystems to debug and build within the teams concept. These subsystems consist of the Microcontroller, Temperature Sensor, Humidity Sensor, and the Motor Controller. Each is an important part for the overall functionality of the design. The Microcontroller will be incharge of communication via web and I2C Channels. The I2C Channels will be in comunication with the Temperature Sensor, Humidity Sensor, and the Motor Controller. The other subsystems will be in communication with the Microcontroller for key operations such as producing an efficient Temperature and Humidity Sensory environment for proper ventilation. The Motor Controller subsystem is in charge of controlling the duration and status of the onboard and present areas ventilation system. Each of these subsystems can be seen bellow in Figures 1 - _. 

<!DOCTYPE html>
<html>
  <head>
    <title>Title of the document</title>
  </head>
  <body>
    <h1>Team PCB Schematic</h1>
    <iframe src="media/314_team_schematic.pdf" width="100%" height="500px">
    </iframe>
  </body>
</html>

<br> 
<p>Above can be seen the teams schematic which possesses all onboard components necessary for the proper function of the design. On the left side of the schematic can be seen the Power Regulator, Pic Microcontroller, and the onboard ESP32 which components are covered by Lukas Severinghaus. On the right side can be seen the Temperature Sensor, built by Carlos Chacon, the Humidity Sensor, built by Miguel Chacon, and the Motor Controller, Built by Wyatte Ricks. The other sections consist of the interactive buttons, debugging LEDS, and connectors for the I2C programming, OLED display, debug UART, and ICSP. </p>

<br>

**Power Regulator, PIC, ESP32:**

The power regulator connected to a micro female usb plug will be using the 
**RT8059GJ5-LJS** to provide a 3.3V supply to low power components. The 5V supply will be used for the Motor Controller, Servo, and Fan motors. This provides an easy power option for users to deal with instead of a bulky block power bank. Power rails will have pull down capacitors for clean current flow through the microchips. 

The PIC which is the main control and communication unit will be connected to all onboard devices. The **PIC24FJ64GA702-LJS** which is connected to vcc has I2C and SPI communication channels. This will be connected with all debugging LEDS, interactive buttons, and connectors such as the I2C programming, OLED display, debuging UART, and ICSP. The PIC will also be interactive through online communication incase users want a more remote option.

The ESP32 is the main communication with online resources for an interactive design for users. This will allow users to be able to read Temperature and Humidity remotely within the designated environment. With the increasing digital interactivity in the daily life this adds a higher customer approval and user friendly option.

<br>

**Temperature Sensor**

For the products design there is an on board Temperature Sensor that will be used for effective ventilation regulation. The **TC74A4-3.3VCTTR** will be in communication with the PIC Microcontroller via I2C channels. The sensor will be simply connected to VCC and equipped with a pull down capacitor. The simplicity of the design will provide a less complex PCB design for the confined space required. This is important as to steer away from a bulky and less appealing design. 

<br>

**Humidity Sensor**

Included with the design will also posses a Humidity Sensor that will be used for effective ventilation. The **HIH6030-021-001** will be in communication with the PIC via I2C Channels. The sensor shares simplicity with the Temperature Sensor in how its design is compact. 

<br>

**Motor Controller**

The Motor Controller is in charge of controlling the fan speed and direction. This **DRV8830DGQR** will be in communications via I2C Channels with the PIC. For proper readings from the Humidity and Temperature Sensor the fan will blow air into the module to provide no interference of onboard temperature and humidity. The fan will then vent the system during operations such as timers and auto mode to reduce moisture within the components. To achieve the best operation for users a simple fan can prove more useful and important for accurate readings and achieve users desires.

<br>

**Cost of Production**

As seen in the team schematic there are a lot of onboard components used for the design and functionality of the product. The production of one component comes out to be approximately $45. This is important as the one of the gaols for our design is to achieve in inexpensive option for customers looking to have a simple instillation process and environmental control unit. All of the on board parts can be fund in [**Appendix C**](appendix-c-billofmaterials) on the home page. The cost seen above on the document is for 1 total unit. 
