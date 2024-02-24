If you need to add +1 temperature sensor for you FLSUN V400 3D printer or another 3D printer with EXP2 slot on his MCU - you can do it by the following way and parts.

Main parts of this setup will be MAX31865 RTD converter + P100 termistor </br>
https://www.aliexpress.com/item/1005006407781161.html </br>
![image](https://github.com/ViktorDiy/FLSUN-V400-extra-temperature-sensor-by-EXP2-slot-plus-MAX31865-RTD-converter/assets/147925158/da7cad7d-1edc-411e-a266-3346f7d45dbc) </br>

We shoul connect MAX31865 with MCU by SPI interface which we have at EXP2 slot. </br>
![Extra PINs correct](https://github.com/ViktorDiy/FLSUN-V400-extra-temperature-sensor-by-EXP2-slot-plus-MAX31865-RTD-converter/assets/147925158/2efb4fd9-5866-44d4-b24e-303d0c9d6979) </br>
![image](https://github.com/ViktorDiy/FLSUN-V400-extra-temperature-sensor-by-EXP2-slot-plus-MAX31865-RTD-converter/assets/147925158/49e8fc11-c520-450e-9f7e-2459e9f9c6cf) </br>
![image](https://github.com/ViktorDiy/FLSUN-V400-extra-temperature-sensor-by-EXP2-slot-plus-MAX31865-RTD-converter/assets/147925158/142316c9-ae49-4dd8-ba25-2486d59fcf1f)</br>

</br>
FLSUN already use some pins of EXP2 for LED head ligth:</br>
EXP2_7 PE12 "output_pin LED_pin" in printer.cfg for head led light</br>
EXP2_9 GND</br>
</br>
So, we can use for extra temp sensor via SPI + MAX31865:</br>
EXP2_1 MISO PA6</br>
EXP2_2 SCK PA5 (clock)</br>
EXP2_6 MOSI PE10</br>
EXP2_4 CS PE0 (temperature signal)</br>
</br>
Very usefull video about MAX31865 and P100/P1000 termistors connection and some solderings on this board for it right configuration:</br>
https://youtu.be/at8T6UYoTt8?si=tq-utT8XKpx-lrK0 </br>
</br>
Please pay your attension that for some MAX31865 boards MOSI-MISO connection  EXP2<->MAX31865 can be direct, but for some opposit. </br>
For MAX31865 board on the picture above it has direct connection MISO (EXP2) -> SDO (MAX31865), MOSI (EXP2) -> SDI (MAX31865) </br>
</br>
For this setup I moved FLSUN LED head slot to external board with MAX31865 </br>
https://www.aliexpress.com/item/1005004266492521.html </br>
https://www.aliexpress.com/item/1005004762590129.html </br>
  
![image](https://github.com/ViktorDiy/FLSUN-V400-extra-temperature-sensor-by-EXP2-slot-plus-MAX31865-RTD-converter/assets/147925158/4a373463-98c3-4d7e-a673-1fac8ed7eeaa) </br>
![image](https://github.com/ViktorDiy/FLSUN-V400-extra-temperature-sensor-by-EXP2-slot-plus-MAX31865-RTD-converter/assets/147925158/8142f2ec-fcc3-49bb-8799-1a9bf57f4728) </br>







