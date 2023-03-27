# BlueRetro Mini ESP32 Devkit C Shield

![image](https://user-images.githubusercontent.com/14284785/228091090-3027bc66-3b5b-45ce-8a4b-27282f3e6bc4.png)

This is part of a game console controller adaptor that works with the [BlueRetro project](https://github.com/darthcloud/BlueRetro), it requires a ESP32 Devkit C and to build HDMI plug to game console wiring adaptors, it looks like this: 
![image](https://user-images.githubusercontent.com/14284785/228091112-598d3384-3fa1-4f86-b990-3d0c2822a0cf.png)

The BRMini uses bidirectional level shifters and a high range power supply to allow the ESP32 to be powered by, and be compatible with, the BlueRetro consoles while only using wired adaptor cables, for example this Adafruit HDMI Plug Breakout Board: 
![image](https://user-images.githubusercontent.com/14284785/228091167-f9456438-55b1-443e-96d5-ebfb532205d0.png) 

and extension cables such as those available on [Aliexpress](https://www.aliexpress.com/w/wholesale-sega-saturn-extension.html).

To wire your own, you should reference the pinouts at the [BlueRetro HW project](https://github.com/darthcloud/BlueRetroHW) DIY section. I suggest to put together two tables to aid wiring as per the below Sega Saturn example:

Identify the player cable and wire colour to console side connection:

![image](https://user-images.githubusercontent.com/14284785/228091208-102d741f-70e8-49da-b38c-91cbec3f5ab6.png)

Identify the appropriate BRMini pin on the HDMI socket:

![image](https://user-images.githubusercontent.com/14284785/228091224-d335558a-9946-4eb0-b58b-b01549aceb20.png)

I have had the project fabricated by JLCPCB as per the gerber files available in this repo.

Wishlist/Goals:
  1. Replace the IC4 level shifter with a smaller one to reduce the cost and improve the footprint (IO39 is primarily for autodetect and has a less stringent requirement)
  2. Integrate the ESP32 onto a single board to remove the need for the devkit and pin headers, ideally reducing the cost (will need to fit the required components and a way to program it.)

The project is licenced under Creative Commons Attribution 4.0 International (CC BY 4.0)
