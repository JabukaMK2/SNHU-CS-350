# SNHU-CS-350
Emerging Sys Arch

### Summary
The final project was to create a thermostat that responded to ambient temperature and took input from three buttons.  Our embedded system was a Raspberry Pi 4B using GPIO and serial bus as the basis for processing.  It also used other embedded systems such as PWM, I2C, and UART.  In this project we finished the build that we had been iterating upon since the start of class.  The end project was about creating a deliverable for the SysTec, then analyzing if the same tech with the same peripherals would suit another embedded system architecture.

### Improvements
The main improvement I would make is the listener on the temp up and down buttons.  Right now, the state machine gets confused if it receives input when it polls because the state machine holds and receives no input for that time.  In some tests, if you spammed the temp up or down button the app would stop receiving input from the up and down button.  I would also add holding the button down to slowly increase or decrease the temperature and have listening on the button that saved inputs that have not yet been processed to process when the state is free.  Last I would add automatic heat and cool controls that enable and disable heat and cool functions when they are needed, instead of just changing the mode between heat and cool.

### Tools
This course gave me strong understanding of GPIO and serial bus communications.  I have several Raspberry Pis, but I must confess that I haven't used the GPIO pins till now.  I also know what I would actually be looking for should I need resources for embedded systems in the future.

### Skills
This project gave me a strong understanding of GPIO bread boards for future use.  The code side also gave me a clearer understanding of the embedded systems that exist around me every day.  I will definitly start my own projects from here, creating new tools to solve problems within my smart home setup.

### Project
The project uses best practices of readable code via whitespace, comments, and modularity in design for future applications.
