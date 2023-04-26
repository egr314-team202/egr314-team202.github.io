# Final Hardware Implementation

Below is the final team PCB schematic showing the temperature, humidity, motor driver, microcontroller, ESP32, and power regulator subsystems. The schematic also shows headers for attaching the OLED, fan, and servo motor.
<body>
    <h1>Final Team PCB Schematic</h1>
    <iframe src="media/314_team_schematic.pdf" width="100%" height="500px">
    </iframe>
  </body>

<body>
    <h1>Final Team PCB Front and Back Design</h1>
    <iframe src="media/314-team-pcb-final.pdf" width="100%" height="500px">
    </iframe>
  </body>

<body>
    <h1>Final Team PCB Front and Back</h1>
    <iframe src="media/314-team-pcb-final.pdf" width="100%" height="500px">
    </iframe>
  </body>

<br>

# PCB Functionality 
The final pcb was designed with the goal of shaping it so that it fits within the size of standard light switch. The dimensions of a standard light switch encasing is 2.75 inches wide and 4.5 inches tall. The team managed to design the pcb so that it is 2.36 inches wide and 3.93 inches tall, thus fitting within the size constraints. 
## Connectors
The pcb also includes several connectors that serve for debugging and programming purposes. These connectors were useful to ensure that there are no shorts, no component are drawing too much current, and that data is being sent via I2C and UART. The connectors located next to the PIC microcontroller allow the microcontroller to be programmed using the PICKit 4 In-circuit debugger. There are also connectors next to the ESP32 for programming it using a USB-to-serial adapter. Right next to to these connectors are four connectors which are for the OLED screen.
<br>

## Buttons
The pcb includes a total of five buttons. Three of which act as interrupts for setting the system into the off, auto, and timer modes. The fourth button is for hard resetting the ESP32 and the fifth button is the boot loader for the ESP32.

## Sensors
The humidity and temperature sensor are located in the bottom right corner of the PCB, which is where the fan controlled using I2C would be located. This would allow the fan to bring in air from the external environment, which would allow the sensors to receive accurate data without affecting the rest of the pcb components.

## Micro USB and Power Regulator
At the bottom left of the pcb is a female micro USB connector with a power regulator, which allows the system to be easily powered with 5V using a micro usb cable and then set down to 3.3V for all the sensors and logic components.

## Motor Driver
Right above the humidity and temperature is the motor driver which runs both the servo motor and the fan. To satisfy project requirements, the motor driver is able ot run both the servo motor and fan and communicate through I2C to control the speed of the fan.