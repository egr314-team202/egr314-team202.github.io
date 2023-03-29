# Product Requirements

Every household has a high levels of water intake at a variety of temperatures according to different applications. With the high levels of heat produced by hot water in confined spaces a leading problem in todays world is the mold produced in these humid environments. Small levels of mold can lead to respiratory problems and allergic reactions. This build up of mold is due to poor ventilation within these spaces with the random intervals of activity present.

## Objective

With this leading problem there in lies our objective to solve this issue. The goal of our project is provide an inexpensive option for controlling high levels of humidity or temperature in effective intervals. Rental users or even customers who are searching to reduce their electrical bills will find this device to be best suited for them as it can be placed over a wall mounted switch to control the already installed ventilation system. 

## Stakeholders

_**Users**_

_**Homeowners**_ - Looking for a way to lower energy costs and mitigate the potential damage caused from humidity and moisture in confined spaces with a solution that can be easily integrated into their current system.

_**Tenants**_ - Looking for a way to connect their home without altering existing wiring, lower energy costs, and prevent potential damages due to humidity and moisture in confined spaces.

_**Bathroom users**_ - Looking for an easy way to turn on the fan for a set period of time, without needing to come back to turn it off.

_**Renters**_ - Looking for a way to reduce overall energy consumption and avoid having to deal with the hassle of humidity and moisture related damages.

_**Use Cases**_

_**User Story #1: Jack**_

Jack is a middle class working father. He has a home automation system installed in his house so that he can monitor it while he is away, as well as stay conscious of his energy usage and utilities spending. He’s comfortable working with basic tools, but is renting the house, so he can’t physically retrofit any switches. He wants to be able to control the fan in his bathroom both to regulate the moisture level and reduce energy wastage. He also wants to be able to monitor the humidity and temperature in real time so that he can display the data on his home automation system.
Jack’s new switch allows him to remotely monitor the environment in the bathroom, and ensure humidity levels don’t build up. The manual override function lets him, or one of his kids, turn it on for a few minutes if needed. Periodic data readings from the switch feed into his home automation system, enabling him to get near-real time updates on humidity and temperature and watch the usage patterns of the fan. He was happy that this device was able to fit on top of the existing switch as it didn’t require him to modify the electrical wiring in the bathroom. With the device having no external moving parts or electrical contacts, he feels safe that it won’t endanger him or his kids.

_**User Story #2: Harlow**_

Harlow is a middle class worker who has child support and groceries to pay for. He has found himself with little to no money after having paid his utility bills and child support. Harlow has therefore started to search for ways to conserve electricity within his home in hopes to lower utility costs. The main areas Harlow spends time in are in his office, bathroom, and living room. Within each of these areas Harlow needs to have light to be able to see what is going on. Harlow is looking for a way to not only dim but effectively keep his home clean and efficient. 
Harlow went onto Amazon and couldn't find anything that could attach to his already installed light switches. With the little money Harlow has left he finds a company whose product can fit right over his current one. Harlow orders one for his bathroom and easily installs it within seconds. After testing the product, Harlow discovers that not only his utility bills lowered over the next month but that his bathroom was smelling fresh and humidity free the whole month. He decided to buy more with the money saved from utilities and now feels more relaxed each month.

# Aspects

With the high valued user needs mentioned in the [User Needs](user-needs) section, the project scope has specific requirements based on these needs. Each sections below takes in consideration the desired user experience but also taking in account safety and overall appealing design. These are important for the design process as it will guide the process of development in the right direction. 

 1. _**Hardware/Product Design**_

    a. The device must survive up to 100% relative humidity in a bathroom environment. <br>
    b. The device must continue to function across a range of operating temperatures.<br>
    c. The device must not require modification to existing wiring or switches.<br>
    d. The device’s electrical components shall be surface mount components.<br>
    e. The device shall have at least one switching voltage regulator.<br>
    f. The device must have at least 1 motor / linear actuator with bidirectional control ability using serial-based (I2C or SPI) motor control<br>

2. _**Software/Functionality**_

    a. The device must communicate using open, documented protocols.<br>
    b. The device must operate with minimal configuration or setup.<br>
    c. The device shall be powered through a wall power supply.<br>
    d. The device shall include a microcontroller with a 8 or 16-bit Microchip PIC families* & ESP32.<br>
    e. The device’s hardware shall be able to successfully communicate with the microcontroller.<br>
    f. The device’s PCB board shall be created using Cadence.<br>
    g. The device’s system level logic shall be 3.3V.<br>
    h. The device shall have at least two serial sensors and one serial actuator using SPI or I2C.<br>
    i. The device must have Board-to-Web duplex communication over WiFi<br>

3. _**Interactivity and User Experience**_

    a. The device’s interface must be intuitive for users of all ages.<br>
    b. The device’s interface must be able to be used in high humidity environments.<br>
    c. The device’s interface should not emit excess light (cost efficient).<br>
    d. The user should be able to configure and integrate the product in a timely manner and without much effort<br>

4. _**Customization**_

    a. The device must be able to be configured. <br>
    b. The device should support remote configuration. <br>
    c. The device should be able to be user color choice supportive.<br>
    d. The device should have parent controls active.<br>
    e. The device software should have one form of UART, SPI, and I2C.<br>

5. _**Manufacturing**_

    a. The device must be manufacturable using the machines available to the design team.<br>
    b. The device must be cost effective to assemble. <br>
    c. The device must be easily repairable.<br>
    d. The device shall not exceed a budget of $240.<br>
    e. The device must have durable parts.<br>

6. _**Safety**_

    a. The device must not present electrical contacts or other hazards to the user.<br>
    b. The device must contain adequate safeguards to prevent overheating, fire, or frying of electrical components.<br>
    c. The device has a safe method to power itself.<br>
    d. The device must not use excess force that might hurt the user or damage the switch<br>

## Milestone dates

Concept presentation: 01/23/2023<br>
Design presentation: 03/01/2023<br>
Design freeze: 03/02/2023<br>
Planned release: 04/28/2023<br>

[Back to Home](index)