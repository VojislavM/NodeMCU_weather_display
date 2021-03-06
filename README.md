# NodeMCU_weather_display [![Build Status](https://travis-ci.org/VojislavM/NodeMCU_weather_display.svg?branch=master)](https://travis-ci.org/VojislavM/NodeMCU_weather_display)
Small WiFi weather display based on NodeMCU

This is a small project to display outside weather conditions. It uses NodeMCU as the main MCU with WiFi and small SSD1306 display. This project is based on [@Mjrovai](https://github.com/Mjrovai) project published as [tutorial on hakster.io](https://www.hackster.io/mjrobot/iot-made-simple-home-weather-station-with-nodemcu-and-oled-27d3a9?ref=explore&ref_id=trending___&offset=3). Difference is that I did not need indoor temperature reading, so the display will only show forecast from the [wunderground](https://www.wunderground.com/) website You can find original firmware on this [repo](https://github.com/Mjrovai/MJRoBot-Home-Weather-Station).

There is a new 3D printable case (STL file) on this repository, folder **case_3D**.

![alt tag](https://github.com/VojislavM/NodeMCU_weather_display/blob/master/Pics/schematics.png)

### Hardware components:
* 1x [NodeMCU](http://nodemcu.com/index_en.html)
* 1x [Adafriud OLED SSD 1306 or compatible](https://www.adafruit.com/product/326)
* 1x USB Power supply

### Firmware (Setup):
* [Arduino IDE](https://learn.sparkfun.com/tutorials/esp8266-thing-hookup-guide/installing-the-esp8266-arduino-addon)

### Note:
* I had the problem with wunderground API to find appropriate City Name and Country "code". My city is "Novi Sad", and it has one white space and two words. If you have the similar city name, with white spaces, use underscore instead of whitespace: "Novi_Sad". Also in the [wunderground international city code list was code](https://www.wunderground.com/about/faq/international_cities.asp) for my country, "Serbia". The code in the list was "YG", but the correct code was "RS", so watch out for that when changing.     

### TODO:
* make new case for nodeMCU
---

#### License

Hardware including documentation is licensed under [CERN OHL v.1.2. license](http://www.ohwr.org/licenses/cern-ohl/v1.2)

Firmware and software originating from the project are licensed under [GNU GENERAL PUBLIC LICENSE v3](http://www.gnu.org/licenses/gpl-3.0.en.html).

Open data generated by our projects is licensed under [CC0](https://creativecommons.org/publicdomain/zero/1.0/legalcode).

All websites and additional documentation are licensed under [Creative Commons Attribution-ShareAlike 4 .0 Unported License] (https://creativecommons.org/licenses/by-sa/4.0/legalcode).

What this means is that you can use hardware, firmware, software and documentation without paying a royalty and knowing that you'll be able to use your version forever. You are also free to make changes but if you share these changes then you have to do so on the same conditions that you enjoy.
