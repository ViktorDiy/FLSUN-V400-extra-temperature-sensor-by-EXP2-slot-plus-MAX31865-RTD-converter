If you need to add +1 temperature sensor for you FLSUN V400 3D printer or another 3D printer with EXP2 slot on his MCU - you can do it by the following way and parts.

Main parts of this setup will be MAX31865 RTD converter + P100 termistor </br>
https://www.aliexpress.com/item/1005006407781161.html </br>
![image](https://github.com/ViktorDiy/FLSUN-V400-extra-temperature-sensor-by-EXP2-slot-plus-MAX31865-RTD-converter/assets/147925158/da7cad7d-1edc-411e-a266-3346f7d45dbc) </br>

We shoul connect MAX31865 with MCU by SPI interface which we have at EXP2 slot. </br>
![Extra PINs correct](https://github.com/ViktorDiy/FLSUN-V400-extra-temperature-sensor-by-EXP2-slot-plus-MAX31865-RTD-converter/assets/147925158/2efb4fd9-5866-44d4-b24e-303d0c9d6979) </br>
![image](https://github.com/ViktorDiy/FLSUN-V400-extra-temperature-sensor-by-EXP2-slot-plus-MAX31865-RTD-converter/assets/147925158/49e8fc11-c520-450e-9f7e-2459e9f9c6cf)
![image](https://github.com/ViktorDiy/FLSUN-V400-extra-temperature-sensor-by-EXP2-slot-plus-MAX31865-RTD-converter/assets/147925158/142316c9-ae49-4dd8-ba25-2486d59fcf1f)</br>

</br>
FLSUN already use some pins of EXP2 for LED head ligth:</br>
EXP2_7 PE12 "output_pin LED_pin" in printer.cfg for head led light</br>
EXP2_9 GND</br>
</br>



