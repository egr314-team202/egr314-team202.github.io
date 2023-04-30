# Final Hardware Implementation

Below is the final team PCB schematic showing the temperature, humidity, motor driver, microcontroller, ESP32, and power regulator subsystems. The schematic also shows headers for attaching the OLED, fan, and servo motor.
<body>
    <h1>Final Team PCB Schematic</h1>
    <iframe src="media/314_team_schematic.pdf" width="100%" height="500px">
    </iframe>
  </body>

<body>
    <h1>Final Team PCB Front and Back Cadence Design</h1>
    <iframe src="media/314-team-pcb-final.pdf" width="100%" height="500px">
    </iframe>
  </body>

<body>
    <h1>Final Team PCB Front and Back Design</h1>
    <iframe src="media/PCB-photos-final.pdf" width="100%" height="500px">
    </iframe>
  </body>
  NOTE: The motor driver pads are covered in soldermask. For the final product, the layer of soldermask was removed from each pad and the motor driver was attached.

<br>

# PCB Functionality 
The final PCB was designed with the goal of shaping it so that it fits within the size of standard light switch encasing. The dimensions of a standard light switch encasing are 2.75 inches wide and 4.5 inches tall. With this size constraint in mind, the team managed to design the PCB so that it is 2.36 inches wide and 3.93 inches tall. The PCB is designed for the user to be able to monitor and control the humidity in a given space. The three buttons going in a straight line on the left side of the board act as interrupts, which allows the user to change the state the system is in. The three states are off, timer, and auto. The off state turns the system off, the timer state sets the fan on for five minutes (increments the timer by five minutes each time the button is pressed and will loop back to zero if the time passes 25 minutes), and the auto state, which will turn the fan on and off when the humidity sensor reads a data value within the set range. As seen in the front photo of the final PCB design, the state buttons were designed to go along a straight line for convenience and to reduce the confusion of each buttons function. 

Another design feature the team decided upon was to integrate the ESP32 into the board rather than attaching a development board to it. The reasoning behind this was that the development board would make the board too big and thus not fit within the space constraints developed in the project requirements.

Furthermore, the team decided to add a female micro usb connector as it would make it much easier to power the board with a micro usb cable rather than a large bulky power supply. It would also be much more convenient for the user. 
## Connectors
The PCB also includes several connectors that serve for debugging and programming purposes. These connectors were useful to ensure that there are no shorts, no component are drawing too much current, and that data is being sent via I2C and UART. The connectors located next to the PIC microcontroller allow the microcontroller to be programmed using the PICKit 4 In-circuit debugger. There are also connectors next to the ESP32 for programming it using a USB-to-serial adapter. Right next to to these connectors are four connectors which are for the OLED screen.
<br>

## Buttons
The PCB includes a total of five buttons. Three of which act as interrupts for setting the system into the off, auto, and timer modes. The fourth button is for hard resetting the ESP32 and the fifth button is the boot loader for the ESP32.

## Sensors
The humidity and temperature sensor are located in the bottom right corner of the PCB, which is where the fan controlled using I2C would be located. This would allow the fan to bring in air from the external environment, which would allow the sensors to receive accurate data without affecting the rest of the pcb components.

## Micro USB and Power Regulator
At the bottom left of the pcb is a female micro USB connector with a power regulator, which allows the system to be easily powered with 5V using a micro usb cable and then set down to 3.3V for all the sensors and logic components.

## Motor Driver
Right above the humidity and temperature is the motor driver which runs both the servo motor and the fan. To satisfy project requirements, the motor driver is able ot run both the servo motor and fan and communicate through I2C to control the speed of the fan. While the motor driver the team chose fit the project requirements and performed well, the team noted that a bigger sized motor driver would be more beneficial the next time as it would be easier to solder the component onto pads of a bigger size.

# Version 2.0

The team did not really experience many difficulties with the current hardware design. The real challenge was finding the time to solder roughly one hundred surface mount components and make sure that all of them were correctly placed on the board. With that said, there are a few improvements that could be made to the hardware design. For starters, we could add the symbol markers to each component on the PCB to better figure out what component goes where. Another improvement would be to shorten the PCB size and stack multiple PCBs on top of each other for a more concise design. The next improvement would be to remove the temperature sensor since the humidity sensor has the capability of also acting as a temperature sensor, which would reduce unnecessary redundancies within the design and make the overall design more cost effective. As seen in the schematic above, there are also several LEDs and connectors added to the design that serve for debugging purposes. While this is great for prototyping, in order to minimize the size of the PCB as much as possible for a more compact design and to reduce the cost for mass production, it would make sense to remove as much of these debugging components as possible for the final product as they would no longer be required.

<br>

# Final Bill of Materials

The final bill of materials is located in Appendix E, which you can get to by clicking on this [link](appendix-e-billofmaterials).

[Back To Home](index)