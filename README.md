# smart-fridge-magnet
Fridge magnet with 4.2" eInk display for HomeAssistant

![Image](https://raw.githubusercontent.com/MarcoFranchi/smart-fridge-magnet/master/IMG_0280%20(2).jpg)
## Bill od Material
* 1 Box prineted in 3D (three pieces)
* 4 Screws M8x12mm 
* 4 Bolts M8
* 4 Neodymium magnets 10x2mm
* 6 Pieces of beryllium copper sheet arround 18x7mm or other thing for battery contact
* 30cm Of electric wire
* 1 eInk display 4.2" [here](https://www.waveshare.com/e-Paper-ESP8266-Driver-Board.htm) or Anazon, ebay, etc.
* 1 ESP8266 Driver Board [here](https://www.waveshare.com/product/displays/e-paper/epaper-2/4.2inch-e-paper.htm) or Anazon, ebay, etc.
* Cyanoacrylate Glue
* Matt white paint (optional if you want a good finishing)
## Build and program it
* Print in 3D the case, frame and cover using .igs or .step file, best choice is ABS
* Install the Fonts (copy all .ttf in ./fonts ESP folder) 
* Copy the display_1.yaml in ESP folder and compile it
* Flash the ESP8266 Driver Board with .bin file using USB

TIP: for installation and test comment the DeepSleep declaration (line 20-24) before comiling otherwise you will wait one hour before you can make other changes.
## Home Assistant configuration
### Install Home Assistant dependence 
* [Garbage Collection](https://github.com/bruxy70/Garbage-Collection) from HACS
* [Google Calendar Event](https://www.home-assistant.io/integrations/calendar.google/) from HA integration
### Edit configuration.yaml
* Merge the display configuration.jaml with your configuration.jaml file or split it in a differten file if you use include files
