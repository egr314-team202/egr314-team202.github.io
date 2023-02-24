# Hardware Proposal

With a big goal in mind the team has been tasked with separate functions within the building process of the product. Each team ember has been given a complex set of parts called subsystems to debug and build within the teams concept. These subsystems consist of the Microcontroller, Temperature Sensor, Humidity Sensor, and the Motor Controller. Each is an important part for the overall functionality of the design. The Microcontroller will be incharge of communication via web and I2C Channels. The I2C Channels will be in comunication with the Temperature Sensor, Humidity Sensor, and the Motor Controller. The other subsystems will be in communication with the Microcontroller for key operations such as producing an effiecient Temperature and Humidity Sensory inviornment for proper ventilation. The Motor Controller subsystem is in charge of controlling the duration and status of the onboard and present areas ventilation system. Each of these subsystems can be seen bellow in Figures 1 - _. 

<figure class="image">
  <div style="text-align: center">
  <img src="media/314_team_schematic.pdf" width="%"><br>
  Figure 1 - Team Schematic 
  </div>
</figure>

<p>Above can be seen the teams schematic which possesses all onboard components nessicary for the proper function of the design. On the left side of the schematic can be seen the Power Regulator, Pic Microcontroller, and the onboard ESP32 which components are covered by Lukas Severinghaus. On the right side can be seen the Temperature Sensor, built by Carlos Chacon, the Humidity Sensor, built by Miguel Chacon, and the Motor Controller, Built by Wyatte Ricks. The other sections consist of the interactive buttons, debugging LEDS, and connectors for the I2C programming, OLED display, debug UART, and ICSP. </p>

<br>

**Power Regulator, PIC, ESP32:**

<p>The power regulator connected to a micro female usb plug will be using the **RT8059GJ5-LJS** to provide a 3.3V supply to low power components. The 5V supply will be used for the Motor Controller, Servo, and Fan motors. This provides an easy power option for users to deal with instead of a bulky block power bank. 

The PIC which is the main control and communication unit will be connected to all onboard devices. The **PIC24FJ64GA702-LJS** which is connected to vcc will have pulldown capacitors for clean power flow and has I2C and SPI communication channels. </p>

