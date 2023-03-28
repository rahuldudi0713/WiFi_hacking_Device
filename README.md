# WiFi_hacking_Device
Hack any wifi with NodeMCU esp8266 Board

I have designed a code that can hack any WiFi credentials using a NodeMCU Board. You just need to make some small changes and upload the code to NodeMCU. Then, you can power up the board.

You have to change the SSID in the code and give the victim's SSID. NodeMCU will create a fake portal for that WiFi. When someone tries to connect to the fake WiFi, they will be prompted to enter their password, which will then be redirected and stored on our web page.

The code also sets up a web portal that can be accessed using the gateway IP that we set in our code. If you search for gatewayIP/ssid, you will be redirected to a page where you can change the victim's SSID according to your needs. If you search for gatewayIP/pass, you will be redirected to a page where you can view the stored password.


Installation (Arduino IDE)


Open your Arduino IDE and go to "File -> Preferences -> Boards Manager URLs" and paste the following link: 

http://arduino.esp8266.com/stable/package_esp8266com_index.json

Go to "Tools -> Board -> Boards Manager", search "esp8266" and install esp8266

Go to "Tools -> Board" and select you board"

Download and open the sketch "WiFi_Captive_Portal.ino"

You can optionally change some parameters like the SSID name and texts of the page like title, subtitle, text body...

Upload the code into your board.

You are done!
