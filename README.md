# autopilot
ESP32 autopilot BLE

This code can be flashed on an ESP32 using the Arduino SDK.
It can be used as a standalone autopilot based on compasss steering. Another method is to download the app:
https://play.google.com/apps/testing/com.sailtactical.autopilot

By downloading this app, the compass, gyro and GPS of the phone will be used. In that case, you only need an ESP32 and a motor driver. Wire the motor driver to the ESP, Connect VCC and Ground as per documentation. Connect pin 33 to motor-driver-left and pin 32 to motor-driver-right. It is

#For use in the arduino SDK V2. 

Go to tools->library manager. Search for ESP32 analogwrite made by Errouaguy and install it
Go to toold->boards manager and search for esp32. Install the esp32 by Espressif Systems.

Create a folder named autopilot_ble.
In this folder, Put all the files (with .ino and .h extension) from the repository.
Open autopilot_ble.ino with the arduino IDE


Select your board (My case DOIT ESP32) and port. If the ESP boards cant be selected. please add ESP to the arduino IDE
Run

Now open te app on your phone. It will search for a bluetooth device called autopilot. When its found, connect to it.
