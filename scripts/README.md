### Header files : 

Header files that contain some essential definitios that are needed by `isp.c`

`clock.h` 
`isp.h`
`data.h`
`usbasp.h`

### Subroutines in seperate files:
`clock.c`

### Makefile

`makefile` : Used to compile and burn .C files 

##### Steps to compile and burn code (Linux):
1). In `makefile`, mention the .C  file you want to compile and burn; PROJECT = <filename>
1). In Linux terminal, enter the command `make`. This will generate the hex file for the .C file you mentioned in the `makefile`.    
2). To burn the code onto the AVR chip, enter in the terminal : `avrdude -p <device_id> -c usbasp -P usb -e -U flash:w:<filename.hex> `

### Others 

`led_blink.c` : A simple test code that blinks a led 7 times a second 

### Main File

`isp.c` : The code that needs to be deployed on the programmer Atmega
`isp.hex` :The hex file corresponding to `isp.c`

