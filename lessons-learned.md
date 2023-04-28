# Lessons Learned
After reflecting on the semester, the team noticed that there were a lot of lessoned learned while working on this project. Additionally, some lessons were learned from the previous iteration of this course that were then implemented into this semester in order to develop a successful product within the given time restraints. This section lists 10 of the most important lessons learned by the team over the course of this semester and implemented from the previous semester. 

## Lesson 1
Keep up with the deadlines. The deadlines are set because they are the optimal times to have finished a task or assignment. Even when a deadline is pushed back, try your best to get that task or assignment finished by that deadline because the time spent past that deadline will be much needed later in the project. For example, having adequate time to complete all of the software debugging is extremely important. 

## Lesson 2
Order your parts and components as soon as possible and make sure that you order many. This was a lesson learned from last semester and implemented in this one. Not having your components can set you back a lot of time, especially because you need them to complete your boards. The sooner you have them, the easier it will be identify problems and to fix them. Ordering multiple components is important in case they break or get lost, and because you will be making multiple boards.    

## Lesson 3
In this course, having good teammates is crucial for success. Make sure to pick teammate that you have good chemistry with, as it will make the project more enjoyable, but also make sure that they are competent, have shared work hours, and have a good learning and professional characteristics. This includes having a good work ethic and having good communication skills.

## Lesson 4
Use the resources available to you for help. There are so many great resources available to help you succeed in this class. If the team had trouble with a concept and process, it would not hesitate to reach out to Professor Aukes, the Teaching Team, the discussion board, other groups and students, and the class website. The website was especially helpful for the team when learning how to use Cadence. Also, making sure that the team's project and exceptions  were clearly communicated to the professor and provided in writing. For example, the team had to make sure to get the correct approval to incorporate a servo motor into the project.

## Lesson 5
Make clear objectives for each assignment. The team would split each task amongst each other in order to simplify the tasks. Making sure everyone knew what they were supposed to be working on gave everyone a sense of purpose on the team, which helped moral but also made each assignment easier in the end.

## Lesson 6
Use every available resource to check your schematic. The team spent a lot of time focusing on optimizing and verifying the schematic. By breaking it into small, easily manageable parts, and by checking it with several TAs and Dr. Aukes, we were able to eliminate most of the big errors in the board. Despite this, one or two small issues still crept through, but we were able to mitigate them by making small changes. 

## Lesson 7
Don't assume that parts will work together by default. The team initially connected the OLED display to the PIC, however we only realized several weeks later that the PIC didn't have a library to drive the display, and that the ESP32 was much better suited to the task. We also didn't know until we tested our PIC that the I2C peripheral was completely different than the one we used previously in the class, so we had to spend significant amounts of time rebuilding the driver. 

## Lesson 8
Optimize time where you can. One specific way we did this was by purchasing our PCB separately, and by also purchasing a solder stencil. Because we didn't have to wait for our board to get batched with other team boards, we received our PCBs a week in advance of the class. Additionally, the solder stencil reduced the amount of time it took to apply solder paste on the pads and assemble the board. Instead of spending 6+ hours to populate the 92 components on our board, the stencil helped reduce this down to 2 hours. 

## Lesson 9
If you see a small error, fix it now. We encountered several issues with sourcing components, but by keeping a close eye on what orders had been placed and where components were, we were able to minimize the delays missing parts could have caused. We also made sure to address every issue in our alpha board in our final team board. We also worked with some other teams who didn't address seemingly small power supply issues early on, and this caused much larger issues farther down the road.  

## Lesson 10
When there's more than one microcontroller, do the hard tasks on the microcontroller that's easiest to program. Our project involved a significant amount of parsing and conversion of data types, like converting MQTT payloads into data for the PIC, and unpacking PIC values for displaying on the OLED screen. By doing most of this work on the ESP32, which was written in Python, we were able to speed up development, instead of writing it in C on the PIC. Micropython makes it a lot easier to manipulate types, dynamically build objects, and interface with hardware than the PIC. Leveraging this helped us have a functional project much earlier on than if we had only used the PIC. 