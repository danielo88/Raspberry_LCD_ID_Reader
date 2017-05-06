# lcd_id
Read Registers on MCUFRIEND UNO shield for WiringPi.   

It's the same outward appearance, but mcufriend has a lot of variations.   
http://domoticx.com/arduino-shield-2-4-tft-lcd-touch/

Many drivers can distinguish in 0x0000 register.   
There is typical driver ID below.   
http://domoticx.com/arduino-library-tft-lcd-shield/

----

Wirering   

|TFT||Rpi/Opi|
|:-:|:-:|:-:|
|LCD_RST|--|Pin#7|
|LCD_CS|--|Pin#3|
|LCD_RS|--|Pin#5|
|LCD_WR|--|Pin#24|
|LCD_RD|--|Pin#26|
|LCD_D0|--|Pin#29|
|LCD_D1|--|Pin#31|
|LCD_D2|--|Pin#33|
|LCD_D3|--|Pin#35|
|LCD_D4|--|Pin#37|
|LCD_D5|--|Pin#32|
|LCD_D6|--|Pin#36|
|LCD_D7|--|Pin#38|
|5V|--|5V|
|GND|--|GND|

build   
git clone https://github.com/nopnop2002/lcd_id   
cd lcd_id   
cc -o lcd_id lcd_id.c -lwiringPi   
sudo ./lcd_id

----

The following indication is an example of ILI9325.

![ili9325](https://cloud.githubusercontent.com/assets/6020549/25771292/e71459de-3288-11e7-9c46-7aa84469b24c.jpg)


The following indication is an example of ILI9342.

![ili9342](https://cloud.githubusercontent.com/assets/6020549/25771295/ff40144e-3288-11e7-84fc-9ceebcd2b1ed.jpg)

