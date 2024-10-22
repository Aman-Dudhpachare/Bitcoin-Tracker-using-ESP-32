# Bitcoin_Tracker_Using_ESP-32
A physical Bitcoin Ticker. For use with Arduino ESP32 board and I2C OLED display.


# Bitcoin Tracker
***FIT ONLY FOR PERSONAL USE***

If you would like to utilize it commercially, please get in contact with me. I'm open to reaching a consensus. 


ESP32 boards can run the Arduino code for Bitcoin Ticker. This ticker shows the price of Bitcoin relative to the US dollar and indicates a rise or fall in the virtual currency. The CoinMarketCap API provides the price information.


# Hardware
* 0.96 Inch OLED Module 12864 128x64 Yellow Blue SSD1306 Driver I2C IIC Serial Self-Luminous Display Board
* ESP32 ESP-32S Development Board

# Wiring Diagram
![wire-diagram](https://github.com/user-attachments/assets/8bc51a01-00f9-4658-bff0-1fc3327fcf76)


# Installation
Connect your ESP32 board to your computer and open `bitcoinTicker.ino` with the Arduino IDE. 

In `Tools > Board` select `DOIT ESP32 DEVKIT V1`.

Select the correct port that your ESP32 is plugged into via `Tools > Port`. If your board isn't showing up, you might need to install some drivers. A Google Search for `ESP32 Drivers` should give you what you need.

Hit the `Verify` button. Install any necessary libraries via `Tools > Manage Libraries`. Below is the list of libraries I used in this project. You should be able to find them pretty quick by typing these into the search bar. All libraries are found in the Arduino Library Manger(`Tools > Manage Libraries`.) No special installation is needed outside of their library.

Libraries Used:
* Adafruit_SSD1306 (For the OLED Display)
* WiFi (For ESP32 onboard WiFi)
* Wire
* HTTPClient (To make requests to CoinMarketCap)
* NTPClinet (Used to get the time for "Last Updated")
* WiFiUdp (Used to get the time for "Last Updated")
* ArduinoJson (Used to process JSON data retreived from CoinMarketCap)

Once everything is verified successfully, hit the `Upload` button. If your OLED is wired up correctly, you should see the screen displaying that it's connecting to your network, then it will show the ticker. 

I am using the MELIFE ESP32 ESP-32S Development Board.

# Usage
Plug Micro-USB into the Arduino and everything should boot up successfully in less than 10 seconds.

# Support You
Whatever you need; questions answered, requests, bugs; make an Issue. I'll get to them as soon as I can.


