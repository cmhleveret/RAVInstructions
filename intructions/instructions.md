# User Manual for the Remote-Controlled Desk Phone for TV and Film Sets

## Overview
This device is a specially designed desk phone primarily intended for use on TV and film sets. It features an LCD display and an ESP32 microcontroller, which allows for remote control via a web interface. The device can be activated on cue as required on set, with a range of variables that can be adjusted to fit the specific needs of a scene or production.

## Hardware Features
- **ESP32 Microcontroller:**  The core of the device enabling WiFi connectivity for remote operations.
- **LCD Display:** Displays the output based on the instructions received from the web interface. It can display numbers and custom text messages.
- **LEDs:** Indicates the device's status.
- **Switch:** Enables toggling between AP (Access Point) and WS (WiFi Station) mode.

## Hardware Images

![](./images/Subject.png)

![](./images/Subject2.png)

## Web interface Images

![](./images/IMG_6890.png)

![](./images/IMG_6891.png)

![](./images/IMG_6892.png)


## Software Features
- **WiFi Connectivity:** Connects to the internet through WiFi, allowing for remote control via a web interface.
- **Web Server:** The ESP32 hosts a web server that enables the users to interact with the device remotely.
- **Remote Control Features:** Users can set variables such as numbers to be displayed, custom messages, duration for messages to be shown, and control the speaker via the web interface.
- **Display Animation:** The device can display an animation on the LCD where a text string appears to be printed incrementally.

## How to Use
1. **Switch Between AP and WS Mode:** The device can operate in two modes - AP (Access Point) mode and WS (WiFi Station) mode. You can toggle between these modes using the switch on the underside of the device, behind the compartment door. In AP mode, the device creates its own WiFi network, while in WS mode, it connects to an existing WiFi network.

2. **Boot the Device:** Power on the device. The device will boot up and display the IP address, password, and SSID on the LCD screen. These details are required to connect to the device.

3. **Connect:**

- **Connect to the Device AP Mode:** Based on the mode, connect your computer or smart device to the same network as the device. If the device is in AP mode, connect to the WiFi network created by the device using the SSID and password displayed on the LCD screen during boot using a mobile phone or laptop - (the passowrd will be 12345678). 

- **Or Connect to the Device WS Mode:** To do this you will first need to connect to the device using the AP mode. Once connected in AP mode you can enter the SSID and password for the netweork you would like the device to connect to (scroll to the bottomm of the page in the web interface). Once you have submitted these variables you can power down the device and switch modes using the switch found behind the compartment door on the underside of the device. The phone will now attempt to connect to the network. Once sucessfully connected it will display the ip address it can be reached on. Using a phone or laptop that is connected to the same network you can reach the device using this ip address.

4. **Access the Web Interface:** Open a web browser and enter the IP address of the device. This will bring up the web interface.

5. **Set Variables:** From the web interface, you can set variables such as the number or custom message to be displayed, the duration for which they are displayed, and the speaker status.

6. **Send Instructions Using web interface toggle switches:** After setting the required variables, send the instructions to the device by toggling the switches for the corresponding display screen on the web interface. The device will act on these instructions, displaying the entered variables on their respecive sreens.


## Troubleshooting
If the device does not respond as expected, consider the following steps:

- **Check Network Connectivity:** Ensure that the device is connected to the network and that you have entered the correct IP address.
- **Reset the Device:** If the device is unresponsive or behaving unexpectedly, try resetting it (button found on the esp32 controller beneath the compartment door on the underside of the device).
- **Refresh the LCD screen:** If the varibales have not updated properly you can toggle the switch for the screen you are having issues with - this will refresh the variables for the display and should fix and display issues.
- **Check the Web Server:** If you can't connect to the web interface, make sure the web server hosted by the ESP32 is running properly.

## Maintenance
The device should be handled with care. Keep it dry and avoid exposure to extreme temperatures. Store it in a safe place when not in use. If a problem cannot be resolved through troubleshooting, get in touch with me.

## Disclaimer
This device is intended for professional use in film and TV production and should only be operated by trained personnel. Ensure to comply with all relevant local and international laws while using the device.