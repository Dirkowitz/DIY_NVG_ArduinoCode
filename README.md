Welcome to the DIY_NVG_ArduinoCode wiki!


* Update Code for the DIY NVG from General Purpose (see video https://www.youtube.com/watch?v=t9H8MNkv4E8&t=1s)

1. First you should try to flash the ESP32 CAM with Arduino IDE. You find many youtube videos (Video example https://www.youtube.com/watch?v=q-KIpFIbRMk)
2. Download all files 
3. Open the code in the folder DIY_NVG in Arduino IDE and try to verify the code in the IDE
4. Install all missing libaries. You can install a few over the IDE browser and other you have to download them manually from the web
> * TFT_eFEX Lib: https://github.com/Bodmer/TFT_eFEX
> * TFT_eSPI: https://github.com/Bodmer/TFT_eSPI
> * TJpg_Decoder: https://github.com/Bodmer/TJpg_Decoder
> * JPEGDecoder: https://github.com/Bodmer/JPEGDecoder

5. You have to change the in the folder "libraries\TFT_eSPI-master" the file User_Setup.h 
6. The Display have the follwing connections then after the exchange
>*Display --  ESP32
>*VCC --  3.3V
>*GND --  GND
>*DIN --  IO13
>*CLK --  IO14
>*CS --  IO15
>*DC --  IO2
>*RST --  IO16


7. If you want to change between left or right side you have to change in the code (file DIY_NVG.ino) in line 89 tft.setRotation(2); to  tft.setRotation(0);

