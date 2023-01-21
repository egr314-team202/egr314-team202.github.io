---
title: Home
---

# Home

Humidity and Temperature Sensing Project

Arizona State University - Polytechnic campus

EGR 314: Embedded Systems Design 2 - Spring 2023

Team 202: Carlos Chacon, Miguel Chacon, Wyatte Ricks, Lukas Severinghaus

Professor Daniel Aukes

January 23, 2023

 
## Introduction

Bathrooms regularly have high levels of humidity and are disposed to different temperatures throughout the day as a result from the water used by faucets, toilets, and baths/showers. For example, toilets on average use between 1.6-7 gallons of water per flush, which amounts to a possible 12,775 gallons of water per year. Similarly, on average, showers in the United States use more than 1 trillion gallons of water per year. That is the equivalent of about 40 million swimming pools. That is a lot of water and with all that water and changes in temperature comes high levels of humidity which can lead to a buildup of black mold, which can have harmful side effects including respiratory problems and allergic reactions. One of the main reasons for the buildup of black mold is poor ventilation in bathrooms that result in a perfect humid and moist environment that allows black mold to thrive.

## Team Organization

After meeting together and discussing each team member's individual goals and outcomes for the course, the team compiled a list combining the top 5 overarching goals:

1. Improve individual skills and understanding of embedded systems
2. Create a design that is visually appealing
3. Develop a design that is practical and meets user needs
4. Focus on intuitive, human-centric interfaces
5. Promote a collaborative and supportive team environment

_Team Charter_

As a result of the collective team goals and outcomes listed above, Team 202’s charter is: to collaborate and support one another in the development and creation of a visually appealing design that implements the team’s skills and knowledge of embedded systems, conforms to user needs, and incorporates an intuitive, human centric interface in order to produce a successful project with a practical application. 

_Mission Statement_

This team’s mission is to design and build a switch retrofit device that uses environmental sensing and embedded systems to provide an economic and health solution to solve the accumulation of moisture in confined spaces.

## User Needs, Benchmarking, and Product Requirements

In order to develop the requirements for the product, the team first analyzed the market for current solutions to the problem of accumulating moisture in confined spaces. A majority of the solutions were smart switches that revolved around bathrooms and smart technologies affecting the ventilation and temperature setting systems. The different solutions were analyzed and their top positive and negative reviews were recorded and then evaluated for explicit or latnent user needs. These user needs would then be used for benchmarking the product. Below are the 5 products that were analyzed along side important information and the user needs that were extracted form the positive and negative reviews. 

**SONOFF NSPanel Wifi Smart Scene Wall Switch**
**Keywords**: Temperature Light Switch
**Search Results Link**: [](/Link)
**Price**: $89.99
**Description**: With a built-in powerful thermostat, you can set different indoor temperatures for different periods of time, and NSPanel will automatically trigger the heating or cooling equipment according to your setting conditions to keep the room at a comfortable temperature.
**Positive Review User Needs**:
-User states product is great for DIY.(latent)
-User states software was unusable. (explicit)
-User states the product had no physical switch to deal with and turned off to save power. (latent)
-User wishes had a proximity sensor to turn off when not present.(latent)
-User states work with custom software.(explicit)
-Customer state assistance is needed.(latent)

**Negative Review User Needs**:
-User Defines Product as unusable and impractical due to incompatibility with outlet blueprint. (explicit) 
-User states the price was too good to be true.(latent)
-User states the product has false advertising and is no better than a normal light switch. (explicit)
-User states switch doesn't dim the lights.(latent)
-User states product has software issues.(explicit)
-User states product has false advertisement.(latent)

**Honeywell Home RPLS740B ECONOswitch 7-Day Solar Programmable Switch**
**Keywords**: Smart Light Switch
**Search Results Link**: [](/Link)
**Price**: $49.99
**Description**:Scheduled programming allows the Econoswitch to turn your home lights and motors on and off automatically, helping you save both time and energy.
**Positive Review User Needs**:
-User describes product as user friendly and easy to install.(Explicit)
-User states interface navigation is easy to understand.(latent)
-User states the product had auto switching features.(Explicit)
-User states the product was easy to install.(latent)
-Customer states the product lasts for a good amount of time.(explicit)
-User states product has a backup battery.(explicit)

**Negative Review User Needs**:
-User states program was not easy to set up and needed a video to understand.(Explicit)
-User states the video guid was not easy to understand.(explicit)
-Customer states product customer care was poor.(Explicit)
-User states the product kept resetting itself.(latent)
-User states the product doesn't work at all.(Latent)
-User states the product is not worth the price.(latent)

**DewStop FS-875-W1 Adjustable Multi Timer Bath Fan Timer Control With Light Control, White**
**Keywords**: bathrrom ffan timer and light switch combo
**Search Results Link**: [](/Link)
**Price**: $44.00
**Description**: This product is a multi timer fan control that includes an adjustable countdown timer and an adjustable minutes per hour timer. The countdown timer allows you to choose how long the fan will run and the minutes per hour timer allows you to turn the fan on every hour. The product includes manual bath fan control for immediate ventilation and manual light control to operate bathroom lighting. The Blue LED indicator light activates to let you know the fan is turned on.
**Positive Review User Needs**: 
-Design should be simple and effective. (Explicit)
-Design should have flexible control settings. (Latent)
-Design should be easy to install. (Latent)
-Design should be simple. (Explicit)
-Design features should be intuitive. (Latent)
-Design should include moisture sensors to optimize fan run time. (Explicit)
-Design should look aesthetically pleasing. (Explicit)
-Design should be easy to install. (Explicit)
-Design should help remove excess moisture from the room. (Explicit)
-Design should be made of corrosive resistant and quality materials. (Latent)
-Design should be easy to operate. (Latent)

**Negative Review User Needs**:
-The design should include flexible control settings. (Explicit)
-The design should be made of quality materials. (Latent)
-The design should have a long lifespan. (Explicit)
-The design should look aesthetically pleasing. (Explicit)
-The design should allow for easy accessibility to the control settings. (Explicit)
-The product should have an efficient delivery process. (Explicit)
-The design features should work as expected. (Explicit)
-The design should be made of high quality materials. (Explicit)

**Brilliant Smart Home Control (1-Switch Panel) — Alexa Built-In & Compatible with Ring, Sonos, Hue, Google Nest, Wemo, SmartThings, Apple HomeKit — In-Wall Touchscreen Control for Lights, Music, & More**
**Keywords**: Smart Switch
**Search Results Link**: [](/Link)
**Price**: $89.99
**Description**: EASY SMART HOME CONTROL FOR EVERYONE: Brilliant touchscreen panels with built-in Alexa make it easy for everyone at home to control popular smart devices, lighting, cameras, locks, thermostats, intercom, scenes and more by simply replacing a light switch.
**Positive Review User Needs**:
-The device is easy to install (explicit)
-The device is adjustable to multiple outlets (explicit)
-The device is aesthetically pleasing (explicit)
-The device works with a variety of different systems and softwares (explicit)
-The device is relatively inexpensive (latent)
-The device incorporates high quality materials (latent)
-The device is easy to setup and install (explicit)
-The device works well with other smart home devices (explicit)
-The device centralizes many smart home devices (latent)
-The device has a seamless installation process and aesthetic (explicit)
-The device incorporates multiple functions (explicit)
-The device is customizable and kid friendly (explicit)

**Negative Review User Needs**:
-Device acts like a physical switch (explicit
-Device incorporates colors (explicit)
-All the device functions work (explicit)
-The device does not require additional devices to properly function (latent)
-The device easily compatible with third party systems (explicit)
-The device is intuitive and incorporates human-centric interface (explicit)
-The device incorporates seamless integration with other devices (explicit)
-The device should be inexpensive (latent)
-The device is intuitive and incorporates human-centric interface (explicit)
-The device works consistently (explicit)
-The device’s wiring is adaptable (explicit)
-The device is easy to use (latent)

**ThermoPro TP49 Digital Indoor Humidity Meter Room Thermometer with Temperature and Humidity Monitor Mini Hygrometer Thermometer**
**Keywords**: humidity meter
**Search Results Link**: [](/Link)
**Price**: $8.99
**Description**: This product is a combined humidity and temperature meter for household use. It has an indicator for current comfort level based on humidity, and updates every 10 seconds. It has a large LCD for easy reading.
**Positive Review User Needs**:
The device needs to be easy to power (latent)
The device needs to be easy to mount (explicit)
The device needs to be easy to read (latent).
The device’s interface should be minimalistic (latent).
The device must be sensitive (latent).
The device should be low cost (latent).

**Negative Review User Needs**:
The device needs to measure precisely (latent).
The device needs to be reliable (explicit).
The device must be able to survive in high humidity environments (latent).
The device needs to communicate its status clearly (latent).
The device must measure accurately (latent).
The device should be easy to handle (latent).

**User Needs Evaluation**
Having gone through different products and customer reviews that target the product statement, Team 202 generated a combined list of User Needs. This list consists of features and needs that customers liked, asked for, or complained about in the product reviews regarding the different multifunction switches above. The generated User Needs can be found below in Figure 1.

**Figure 1 - Preliminary User Needs**

The next step was to group the user needs into separate categories to develop overarching need statements. The groups can be found in the below Figure 2 and the overarching need statements are highlighted in yellow.

**Figure 2 Organized User Needs**

Once the User Needs were sectioned off into different categories as seen in Figure 2, each User Need was then ranked from Least Important to Most Important. This ranking can be found in Figure 3.

**Figure 3 Ranked User Needs where: ⭐⭐⭐ - Most Important; ⭐⭐ - Important; ⭐ - Least Important**

User Needs List:
1. Interface
⭐⭐⭐Friendly user interface
⭐⭐⭐Incorporates human centric interfaces
⭐⭐Built in timer for display
⭐⭐Gauge readout of humidity
⭐Touch display
2. Customer Support
⭐⭐⭐Good customer care
⭐⭐⭐Helpful/detailed manual/instructions
⭐⭐Easy to read
⭐⭐Communicate status clearly
⭐⭐Time warranty is reasonable
⭐Short delivery process
3. Age friendly
⭐⭐⭐Kid friendly
⭐⭐⭐Safe for inexperienced users
⭐⭐⭐Child proof
4. Intuitive to operate
⭐⭐⭐Simple design functionality
⭐⭐ Multi functional
⭐⭐Intuitive
⭐Acts like a physical switch
5. Cost
⭐⭐Relatively inexpensive
⭐Low cost
6. Reliability
⭐⭐⭐Accurate sensory data
⭐⭐⭐Effective sensors
⭐⭐⭐Device’s functions work
⭐⭐⭐Works consistently
⭐⭐⭐Sturdy design to protect electronic components
⭐⭐⭐Incorporates high quality materials
⭐⭐⭐Moisture resistant
⭐⭐Cold resistant
⭐⭐Heat resistant
⭐⭐Long lifespan
⭐Durable
⭐Wind resistant
⭐Survive high humidity
⭐Corrosive resistant
7. Interoperability
⭐⭐⭐Easy access to control settings
⭐⭐⭐Does not require additional devices to properly function
⭐⭐⭐Wiring is adaptable
⭐⭐Easily compatible with third party systems
⭐⭐Works with a variety of different systems and softwares
⭐⭐Compatible with non-Alexa items
⭐⭐Remote activation
⭐Bluetooth capabilities
⭐LoRa
⭐Compatible with Alexa
8. Energy Efficient
⭐⭐⭐Low power needed
⭐⭐Eco-friendly
⭐Auto switch
9. Measurement features
⭐⭐⭐Timer functionality
⭐⭐⭐Measure precisely, accurately, and sensitively
⭐⭐Motion detection
⭐Pressure measurement
⭐Presence detection
10. Easy to use
⭐⭐⭐Fits standard size wall switch outlet
⭐⭐⭐Easy to mount
⭐⭐⭐Easy to install
⭐⭐⭐Easy to power
⭐⭐Easy to handle
⭐⭐Easily integratable
⭐Easy to program (if required)
⭐Easy to set up
11. Customizable
⭐⭐⭐Adjustable to multiple outlet types
⭐⭐⭐Incorporates multiple functions
⭐⭐Easily removable
⭐⭐Flexible control settings
⭐⭐Multiswitch control
⭐Adhesive mount
⭐Keyhole mount
⭐Magnet mount to switch
12. Aesthetically pleasing
⭐⭐⭐Color blends with the rest of the bathroom
⭐⭐⭐Low profile
⭐⭐⭐Uncluttered interface
⭐⭐⭐Aesthetically pleasing
⭐⭐⭐Modern and slim
⭐⭐Lightweight
⭐⭐Not bulky
⭐⭐Color variations
⭐Incorporates colors

**Product Requirements**
Once the team grouped, sorted, and ranked the variety of user needs that were drawn from costumer reviews of existing products into overarching needs, they were converted into requirements that the product will have to follow. The requirements were divided up into 6 categories:

1. Hardware/Product Design
2. Software/Functionality
3. Interactivity and User Experience
4. Customization
5. Manufacturing
6. Safety

The requirements that were converted from the user needs were then sorted into their respective requirement category and then further defined as seen below.

**Hardware/Product Design**
a. The device must survive up to 100% relative humidity in a bathroom environment. 
b. The device must continue to function across a range of operating temperatures.
c. The device must not require modification to existing wiring or switches.
d. The device’s electrical components shall be surface mount components.
e. The device shall have at least one switching voltage regulator.
f. The device must have at least 1 motor / linear actuator with bidirectional control ability using serial-based (I2C or SPI) motor control
**Software/Functionality**
a. The device must communicate using open, documented protocols.
b. The device must operate with minimal configuration or setup.
c. The device shall be powered through a wall power supply.
d. The device shall include a microcontroller with a 8 or 16-bit Microchip PIC families* & ESP32.
e. The device’s hardware shall be able to successfully communicate with the microcontroller.
f. The device’s PCB board shall be created using Cadence.
g. The device’s system level logic shall be 3.3V.
h. The device shall have at least two serial sensors and one serial actuator using SPI or I2C.
i. The device must have Board-to-Web duplex communication over WiFi
**Interactivity and User Experience**
a. The device’s interface must be intuitive for users of all ages.
b. The device’s interface must be able to be used in high humidity environments.
c. The device’s interface should not emit excess light (cost efficient).
d. The user should be able to configure and integrate the product in a timely manner and without much effort
**Customization**
a. The device must be able to be configured. 
b. The device should support remote configuration. 
c. The device should be able to be user color choice supportive.
d. The device should have parent controls active.
e. The device software should have one form of UART, SPI, and I2C.
**Manufacturing**
a. The device must be manufacturable using the machines available to the design team.
b. The device must be cost effective to assemble. 
c. The device must be easily repairable.
d. The device shall not exceed a budget of $240.
e. The device must have durable parts.
**Safety**
a. The device must not present electrical contacts or other hazards to the user.
b. The device must contain adequate safeguards to prevent overheating, fire, or frying of electrical components.
c. The device has a safe method to power itself
d. The device must not use excess force that might hurt the user or damage the switch


**Bold Text**
_Italic Text_
**_Bold and Italic Text_**

## Research Question

* Bullet Point 1
* Bullet Point 2
* Bullet Point 3

## Background

![image caption](https://idealab.asu.edu/assets/images/research/jumper1.png)

[link to background](/background)

## Results

1. Numbered Point 1
1. Numbered Point 2
1. Numbered Point 3

## Conclusions and Future Work

## External Links

[example link to idealab](https://idealab.asu.edu)


## References
