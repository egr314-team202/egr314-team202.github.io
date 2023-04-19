# Block Diagram
The block diagram helps to visualize and understand how all of the individual subsystem and passive components work and align together with the micro-controller. It is a simple first step before creating the individual and team schematics. 

### Current Block Diagram
<figure class="image">
  <div style="text-align: center">
  <iframe src="media/Team_202_Block_Diagram.pdf" width="100%" height="500px"></iframe> 
  <br>
  Figure 1 - Team 202 Block Diagram
  </div>
</figure>

## Individual Subsystems
The individual team subsystems found in the Block Diagram can be located within the dashed boxes containing the team member's name highlighted in yellow. The following explanations will determine how and why each subsystem satisfies [project requirements](team-organization).

# Microcontroller and Power Regulator
The [PIC24FJ64GA702](component-selection) microcontroller selected for this project has all of the I2C, GPIO, UART, WIFI, ESP32, and ICSP pins and features required to successfully run the final product. The power regulator project requirements are that the final board must include a switching voltage regulator. The selected voltage regulator, [RT8059GJ5](component-selection) satisfies this requirement as it is a 3.3V switching voltage regulator that will be used to provide voltage to the two serial sensors implemented in the project.

# Temperature Sensor
The project requires the product to sense at least two different environmental conditions through at least two separate serial sensors. This subsystem will incorporate a surface mount [TC74](component-selection) temperature sensor which will sense at least one of those environmental conditions (temperature).

# Humidity Sensor
With respect to the same project requirement described above, this subsystem will incorporate an [HIH6030-021-001](component-selection) humidity sensor which will sense the second required environmental condition (humidity).

# Motor Driver and Motors
The project requirements with respect to the motors is that there needs to be at least one motor/serial actuator that is controlled by a motor controller communicating over SPI or I2C-based protocol. For product functionality, a [servo motor](component-selection) was incorporated into the project with verbal and written confirmation from Dr. Aukes. However, to satisfy project requirements and to get more accurate sensor readings by keeping moisture out of the board, a fan, [OD4010-05HB](component-selection), will be used to apply variable speed control and direction for dependent states of the sensors present within the system through I2C protocol, therefore satisfying the project requirements. The selected motor driver, [DRV8830DGQR](component-selection), is able to run both the servo motor and fan and communicate through I2C in order to satisfy the project requirements.

[Back to Home](index)