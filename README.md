# CS-350

## Projects
1. Thermostat
2. SOS morse code

## Summary:

In summary these two projects required taking the TI SimpleLink Wi-Fi CC3220S microcontroller LaunchPad dev kit and creating a thermostat and a blinking light to signal morse code useing the different I2C and RTOS functions. For this I will start with the thermostat as it was the biggest project and required more time than the other project did. In this project we wanted to build a basic thermostat that would read the ambient tempature and depending on our set point. If the tempature was lower than the set point then we would turn on the red LED which would show that the heat was turned on. Once the tempature reached the desired set point then the red LED would turn off signaling the heat was off. We used UART to simulate sending this information to the cloud and printing this information out on a console. <br>
The morse code project was a bit simpler where we utilized I2C again but this time just for button recognition. The objective of this project was to set the LEDs to blink in intervals to represent morse code. <br>
```
Dot = red LED on for 500ms
Dash = green LED on for 1500ms
3*500ms between characters (both LEDs off)
7*500ms between words (both LEDs off), for example SOS 3500ms SOS
```
With this timing we should signal SOS and when a button is pressed it should wait until the sequence is done give us a confirmation, for this I used the yellow LED to blink to confirm the change, and then it should switch to OK in morse code. 
## Things I learned from these:
Some of the things I learned from these projects is how to structure my code and to really pay attention to memory usage. In embedded systems memory managment is key because we have so few resources. I also learned that it is better to spend more time on the design than to stress about how you are going to code it. If you make a well drawn out design and actually understand that design then you will better understand what you need to do to produce the outcome that you want. These are also skills I feel like I could improve better on. Documentation is very important in our field. With proper documentation then even someone that is not as technical should be able to understand how the product works. Clear documentation also allows other developers to understand what we were trying to accomplish so that they might be able to edit or improve the source later on. This also goes to keeping your code clean and well commented. Using proper code structure and good comments allows other developers to read your code which helps keep it maintainable and more adaptable. 

## Tools and resources
The main tool that was used was the code composer studio, but the main resources that I will take from this is the documentation of the embedded boards. While being taksed to look up other boards it showed me how to look at product documentation that tells all the information about the product such as ram to the number of UART pins ect. 
