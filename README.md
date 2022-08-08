# home-remote

I have used the FireBeetle ESP32 board along with a LiPo cell to power the device. Modify the code to fit your needs.

#In progress
1. Battery monitoring
2. WiFi singal strength icon
3. Improve documentation

#Future goals
1. Case
2. Custom PCB design
3. Wireless charging

#Wiring

Buttons:
 I have used the internal pull-up feature of the ESP32 to minimise the number of components and the complexity of the circuit.
 
|    GPIO PIN   |    Button  |
| ------------- | ------------- |
| 23  | Up  |
| 27  | Down  |
| 25  | Right |
