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

## Configuration

 I have added subtitutions for all the entities so that it is much easier to get everything up and running. The remote currently consists of 3 pages: Lights, Home page and Media. Edit the entitiy ids to suit your setup.

### Lights

 Currently you can add 4 lights.
 
![lights](https://user-images.githubusercontent.com/61015809/184081712-5a653ab1-6741-4ff8-bec6-be3b27e2e11e.jpg)

```
#Lights
#Entity ids for lights
  light_1: light.bedroom_lamp 
  light_2: light.bathroom_bulb 
  light_3: light.kitchen_bulb 
  light_4: light.living_room_bulb
#Titles for lights
  light_1_title: Bedroom 
  light_2_title: Bathroom 
  light_3_title: Kitchen 
  light_4_title: Livingroom    
}
```

### Home

 Add a temprature sensor and weather enitiy. The scenes are handled by an input select that contains all the scenes.

![home](https://user-images.githubusercontent.com/61015809/184081731-b45fa0ca-5625-4151-a029-35d6c25867c7.jpg)

```
#Home page
  temprature_sensor: sensor.bathroom_temperature 
  weather: weather.home 

  scenes: input_select.scenes
```

### Media

 Almost any media player in home assistant should work.
 
![media](https://user-images.githubusercontent.com/61015809/184081761-c170ef2b-8aae-4c12-a11a-e940b22eac93.jpg)

```
#Media
  media: media_player.adityas_bedroom
```
### Fonts

 Place all the fonts in "fonts" folder inside the esphome folder.
 
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
 
Your support will help me make more cool projects just like this one :-)

<a href="https://www.buymeacoffee.com/adityapattiyeri" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>



