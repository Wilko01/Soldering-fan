# ..
..

## Description and operation instructions
..

 ## Technical description
.

### Parts
1 x NodeMCU

<img src="Images/ESP8266_NodeMCU.jpg" alt="drawing" width="500"/>

1 x Relay LY2N-J

<img src="Images/LY2N-J_Relay.jpg" alt="drawing" width="150"/>

1 x Relay socket PTF08A

<img src="Images/PTF08A_Socket.jpg" alt="drawing" width="200"/>

Relay socket pinout

<img src="Images/Relay_PTF08A_Socket_pinout.jpg" alt="drawing" width="200"/>

1 x 10k resistor as pull down resistor


### Schematic overview
<img src="Images/Schematic_overview.jpg" alt="drawing" width="500"/>
 
•	Connect the 230V side of the relay according to the installation instructions of the boilerNodeMCU with. See the relay socker pinout below on how to connect.

•	Connect the relay contact to the 3,3V of the NodeMCU and the other side to D6.

•	Connect the 10k resistor to D6 and to GND to use it as a pull down resistor.

### ESPEasy installation
See the instructions in 'Arduino projects and programming' (not listed here)


### ESPEasy Configuration
Check the screenshots for the configuration.

![ESPEasy Config](Images/ESPEasy_Config.jpg)

![ESPEasy Controller](Images/ESPEasy_Controller.jpg)

![ESPEasy Devices](Images/ESPEasy_Devices.jpg)

Pay attention to the Pullup and inverse as there were issues even with the external pulldown resistor.
Additionally when using relais make sure to set a debounce value to make sure that the contacts of the relais don't mess with the state.
![ESPEasy Devices ESPEasy_Switch](Images/ESPEasy_on_off.jpg)

### Interface
#### Home Assistant
Home Assistant is connected via the MQTT broker.

### Testing
.

### Information
- [Rules syntax](https://espeasy.readthedocs.io/en/latest/Rules/Rules.html)

Generic
- [Markdown Cheat Sheet](https://www.markdownguide.org/cheat-sheet/)


### Problems
..

### Wishlist
..


### Code
#### Rules Set 1 without annotation

#### Rules Set 1 including annotation
```
..
```
