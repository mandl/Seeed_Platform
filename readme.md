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
* RePhone Series

Thanks to the new features of Arduino IDE, it's easy to add those board to your Arduino IDE now.

There're few step to be followed. 

##Step 1. Download the latest Arduino IDE

You need a Arduino IDE that after version 1.6.4, please download one if there's no Arduino IDE in your computer.

[![](https://raw.githubusercontent.com/SeeedDocument/Seeeduino_Stalker_V3_1/master/images/Download_IDE.png)](https://www.arduino.cc/en/Main/Software)

##Step 2. Setting your Arduino IDE

Open your Arudino IDE, click on **File > Preferences**, and copy below url to *Additional Boards Manager URLs*

```

https://raw.githubusercontent.com/mandl/Seeed_Platform/master/package_seeeduino_boards_index.json
```

![](https://raw.githubusercontent.com/Seeed-Studio/Seeed_Platform/master/img/settings.png)

##Step 3. Board Manager

Click on **Toos > Board > Board Manager**.

![](https://raw.githubusercontent.com/Seeed-Studio/Seeed_Platform/master/img/board_manager.png)

You will get many board that named with Seeed xxxx, let's take Seeeduino Stalker V3 as example.

Click Seeeduino Stalker V3 then an **Install** button appear, click on it to finish the step, this process takes about 5 minutes to half an hour, which depend on the speed of your network. 

![](https://raw.githubusercontent.com/Seeed-Studio/Seeed_Platform/master/img/add_board.png)

##Step 4. Select a board

After Step 3 was successful, a board named Seeeduino Stalker V3 will show up at the boards list. 

Click on **Tools > Board**, *Seeeduino Stalker V3* is available now. 

![](https://raw.githubusercontent.com/Seeed-Studio/Seeed_Platform/master/img/stalker_board.png)


