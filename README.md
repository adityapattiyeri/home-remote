# home-remote

I have used the FireBeetle ESP32 board along with a LiPo cell to power the device. Modify the code to fit your needs.

## In progress
1. Battery monitoring
2. WiFi singal strength icon
3. Improve documentation

## Future goals
1. Case
2. Custom PCB design
3. Wireless charging

## Wiring

### Buttons:
 I have used the internal pull-up feature of the ESP32 to minimise the number of components and the complexity of the circuit. Connect one end of the button to ground and the other end to the corresponding pin.
 
|    GPIO PIN   |    Button  |
| ------------- | ------------- |
| 23  | Up    |
| 27  | Down  |
| 25  | Right |
| 19  | Left  |
| 26  | Ok    |
| 03  | Home  | 
| 18  | Lights|
| 13  | Media |

### Battery:
 I have used a 1000 mAh LiPo battery directly connected to the FireBeetle board. The board comes with built in battery protection circuit.
 
## The prototype:
### Top:
![top](https://user-images.githubusercontent.com/61015809/183344750-e4a14b74-f6ff-4278-90d3-0384292a35ff.jpg)

### Side:
![side](https://user-images.githubusercontent.com/61015809/183344842-3e42db34-14ed-4ed5-bbbf-0473fe78d72d.jpg)

### Bottom:
![bottom](https://user-images.githubusercontent.com/61015809/183344887-62441bc4-9444-436b-a218-3bacfc54f323.jpg)


<a href="https://www.buymeacoffee.com/adityapattiyeri" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>



