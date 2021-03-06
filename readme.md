[![](http://statics3.seeedstudio.com/assets/img/wiki/wiki_banner_20161013.jpg)](http://www.seeedstudio.com)

Seeed had designed so many boards that work with Arduino IDE, include,

* Seeeduino V3/4
* Seeeduino Stalker V2/3/3.1
* Seeeduino Lite
* Seeeduino Lotus
* Seeeduino Mega
* Seeeduino LoRaWAN/GPS
* Seeeduino GPRS
* Seeeduino Ethernet
* LinkIt ONE
* **RePhone Series**

Thanks to the new features of Arduino IDE, it's easy to add those board to your Arduino IDE now.

There're few step to be followed. 

## Step 0. Install Python3

You need Python   https://www.python.org/ 

and 

pySerial  https://pythonhosted.org/pyserial/pyserial.html

Add your user to dailout group.

	sudo adduser $USER dialout


Install  udev rule under **/etc/udev/rules.d/** called **71-rephone.rules**.
The magic job is here setting ID_MM_DEVICE_IGNORE environment value to inform ModemManager to skip device.


	ATTRS{idVendor}=="0e8d" ATTRS{idProduct}=="0003", ENV{ID_MM_DEVICE_IGNORE}="1"
	ATTRS{idVendor}=="0e8d" ATTRS{idProduct}=="0023", ENV{ID_MM_DEVICE_IGNORE}="1"



## Step 1. Download the latest Arduino IDE

You need a Arduino IDE that version 1.8.3, please download one if there's no Arduino IDE in your computer.

[![](https://raw.githubusercontent.com/SeeedDocument/Seeeduino_Stalker_V3_1/master/images/Download_IDE.png)](https://www.arduino.cc/en/Main/Software)

## Step 2. Setting your Arduino IDE

Open your Arudino IDE, click on **File > Preferences**, and copy below url to *Additional Boards Manager URLs*

```

https://raw.githubusercontent.com/mandl/Seeed_Platform/master/package_seeeduino_boards_index.json
```

![](https://raw.githubusercontent.com/Seeed-Studio/Seeed_Platform/master/img/settings.png)

## Step 3. Board Manager

Click on **Toos > Board > Board Manager**.

![](https://raw.githubusercontent.com/Seeed-Studio/Seeed_Platform/master/img/board_manager.png)


Click  **Install** button appear, click on it to finish the step, this process takes about 5 minutes to half an hour, which depend on the speed of your network. 


![](https://raw.githubusercontent.com/mandl/Seeed_Platform/master/img/install_rephone.png)



## Step 4. Flash firmware. 

### From terminal

	cd ./.arduino15/packages/Seeeduino/tools/linkit_tools/1.1.21
	./firmwareUploader.py 

Switch off Rephone and connect to USB.

### Or using the IDE


Select the *Rephone Firmware Updater*

![](https://raw.githubusercontent.com/mandl/Seeed_Platform/master/img/Firmware1.png)


Select *Burn Bootloader*
Switch off Rephone and connect to USB.

![](https://raw.githubusercontent.com/mandl/Seeed_Platform/master/img/Firmware2.png)

Wait for *Update done*

![](https://raw.githubusercontent.com/mandl/Seeed_Platform/master/img/Firmware3.png)


## Step 5. Select a board

After Step 3 was successful, a board named Rephone core 2G MT2502 will show up at the boards list. 

Click on **Tools > Board**, *Rephone core 2G MT2502* is available now. 

![](https://raw.githubusercontent.com/mandl/Seeed_Platform/master/img/boards.png)


## Set 6. Select port

Select the port **/dev/ttyACM0** und upload your sketch.

![](https://raw.githubusercontent.com/mandl/Seeed_Platform/master/img/port.png)


Open the serial monitor.

![](https://raw.githubusercontent.com/mandl/Seeed_Platform/master/img/SerialMon.png)





