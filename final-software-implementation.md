# Final Software Implementation

## Updated Software State Flow Diagram
Below is the updated software diagram reflecting the final design. There were a few small changes between our initial and final diagrams, but overall the core remained the same. One of the biggest changes was moving the OLED to be connected to the ESP32, instead of the PIC. This reduced the computational load on the PIC and simplified the software for this. 

<iframe src="media/Final-Software-Proposal.pdf" width="100%" height="500px"></iframe>

## Software State Flow Function
Breaking down each of the sections from the above diagram, the main loop forms the core of the decision logic, see figure X.1. After initializing the peripherals and variables, see Figure X.2, it enters an infinite loop.

In this loop, first the temperature and humidity sensors are polled, then a state machine runs the processing function for the current mode. There are three system modes. Off mode leaves the switch in the off position and the fan in the slow speed. Timer mode leaves the switch and fan on for a set amount of time. Auto mode automatically turns on the switch and fan based on the current measured humidity. 

After processing the state functions, the loop also checks for new inbound serial data. The serial commands can either contain a mode command, to switch to a new mode, or a timer command, to set the timer to a specific time. Once this process is complete, the loop begins again.
 
<figure class="image">
  <div style="text-align: center">
  <img src="media/Final-SW-Main.JPG" width="50%"><br>
  Figure X.1 - Main System
  </div>
</figure>

<figure class="image">
  <div style="text-align: center">
  <img src="media/Final-SW-Init.JPG" width="50%"><br>
  Figure X.2 - Initialization
  </div>
</figure>

The state functions have already been touched on briefly, but they implement the logic of each mode. The auto mode contains the main controller logic, which implements a bang bang controller with hysteresis. The hysteresis ensures the controller doesn't oscillate around the humidity setpoint. 

<figure class="image">
  <div style="text-align: center">
  <img src="media/Final-SW-State.JPG" width="50%"><br>
  Figure X.3 - State Functions
  </div>
</figure>

To ensure the system responds promptly, user inputs are processed via interrupt service routines (ISR), attached in the main loop startup. These ISRs get called whenever a button is pressed, and call the necessary logic to change modes or increment the timer. 

One final ISR is called on a 1Hz timer and it serves to count down the clock in timer mode, and send updates to the ESP32. This ensures that MQTT gets updated consistently and that the information on the screen is up to date. 

<figure class="image">
  <div style="text-align: center">
  <img src="media/Final-SW-ISR.JPG" width="50%"><br>
  Figure X.r - Interrupt Service Routines
  </div>
</figure>

## Changes to software design
1) Simplification of the inbound serial protocol.
2) Moving the OLED display from the PIC to the ESP32.
3) Moving the servo. 
4) Incrementing time behavior. 
5) Controller hysteresis.

## Future potential changes

## MQTT Topic Table
We developed the below topic table to document the specific topics used to publish data and receive commands from MQTT. 

<iframe src="media/Final-Topic-Table.pdf" width="100%" height="500px"></iframe>

## C Source Code
Below are all the source files used for the PIC code:
### Main file
<script src="https://emgithub.com/embed-v2.js?target=https%3A%2F%2Fgithub.com%2Fegr314-team202%2Fproject-code%2Fblob%2Fmain%2Fpic%2FTeam202-PIC-Code%2FTeam202-PIC-Code.X%2Fmain.c&style=default&type=code&showBorder=on&showLineNumbers=on&showFileMeta=on&showFullPath=on&showCopy=on"></script>

### I2C Driver
We had to modify code we found to build an I2C driver for the PIC24 as it was not compatible with the existing I2C examples we had.
<script src="https://emgithub.com/embed-v2.js?target=https%3A%2F%2Fgithub.com%2Fegr314-team202%2Fproject-code%2Fblob%2Fmain%2Fpic%2FTeam202-PIC-Code%2FTeam202-PIC-Code.X%2FeepromI2C.c&style=default&type=code&showBorder=on&showLineNumbers=on&showFileMeta=on&showFullPath=on&showCopy=on"></script>
<script src="https://emgithub.com/embed-v2.js?target=https%3A%2F%2Fgithub.com%2Fegr314-team202%2Fproject-code%2Fblob%2Fmain%2Fpic%2FTeam202-PIC-Code%2FTeam202-PIC-Code.X%2FeepromI2C.h&style=default&type=code&showBorder=on&showLineNumbers=on&showFileMeta=on&showFullPath=on&showCopy=on"></script>

### Project Functions
Most of our main functionality is abstracted into the project functions files, to keep the `main.c` file clean.
<script src="https://emgithub.com/embed-v2.js?target=https%3A%2F%2Fgithub.com%2Fegr314-team202%2Fproject-code%2Fblob%2Fmain%2Fpic%2FTeam202-PIC-Code%2FTeam202-PIC-Code.X%2Fproject_functions.h&style=default&type=code&showBorder=on&showLineNumbers=on&showFileMeta=on&showFullPath=on&showCopy=on"></script>
<script src="https://emgithub.com/embed-v2.js?target=https%3A%2F%2Fgithub.com%2Fegr314-team202%2Fproject-code%2Fblob%2Fmain%2Fpic%2FTeam202-PIC-Code%2FTeam202-PIC-Code.X%2Fproject_functions.c&style=default&type=code&showBorder=on&showLineNumbers=on&showFileMeta=on&showFullPath=on&showCopy=on"></script>