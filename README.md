# <a href="https://cooltext.com"><img src="https://images.cooltext.com/5626291.png" width="946" height="144" alt="LRRAAJLS-Raspberry-Team" /></a>


 <a href="https://cooltext.com"><img src="https://images.cooltext.com/5626292.png" width="417" height="83" alt="Sistemas programables" /></a>

 <a href="https://cooltext.com"><img src="https://images.cooltext.com/5626293.png" width="214" height="79" alt="37 Sensor KIT" /></a>



<a href="https://cooltext.com"><img src="https://images.cooltext.com/5626294.png" width="219" height="93" alt="Joystick" /></a>
  ### Codigo
  ```from machine import Pin, ADC
from time import sleep

VRX = ADC(Pin(27))
VRY = ADC(Pin(26))
SW = Pin(22,Pin.IN, Pin.PULL_UP)

while True:
    xAxis = VRX.read_u16()
    yAxis = VRY.read_u16()
    switch = SW.value()
    
    print("X-axis: " + str(xAxis) + ", Y-axis: " + str(yAxis) + ", Switch " + str(switch))
    if switch == 0:
        print("Se presiono el boton!")
    print(" ")
    sleep(2)
```
  ### Corrida
  
  ### Imagenes del circuito
  
 
 
<a href="https://cooltext.com"><img src="https://images.cooltext.com/5626295.png" width="179" height="79" alt="Flame" /></a>
  ### * Codigo
  ```from machine import Pin
import utime

flame_sensor = Pin(16, Pin.IN)
utime.sleep(2)

while True:
   if flame_sensor.value() == 1:
       print("Flame Detected")
       utime.sleep(3)
   else:
       print("No Flame")
       utime.sleep(1)
utime.sleep(0.1)```

  ### * Corrida
  
  ### * Imagenes del circuito
  
  
## <a href="https://cooltext.com"><img src="https://images.cooltext.com/5626297.png" width="230" height="48" alt="RGB LED" /></a>
  ### * Codigo
  
  ### * Corrida
  
  ### * Imagenes del circuito
  
  
## Heartbeat
  ### * Codigo
  
  ### * Corrida
  
  ### * Imagenes del circuito
  
## Light cup
  ### * Codigo
  
  ### * Corrida
  
  ### * Imagenes del circuito

## Hall Magnetic
  ### * Codigo
  
  ### * Corrida
  
  ### * Imagenes del circuito
  
 
## Realy
  ### * Codigo
  
  ### * Corrida
  
  ### * Imagenes del circuito
  
## Linear Hall
  ### * Codigo
  
  ### * Corrida
  
  ### * Imagenes del circuito
  
## SMD RGB
  ### * Codigo
  
  ### * Corrida
  
  ### * Imagenes del circuito
  
## Color Flash

  ### * Codigo
  
  ### * Corrida
  
  ### * Imagenes del circuito
  
## Tilt switch

  ### * Codigo
  
  ### * Corrida
  
  ### * Imagenes del circuito
  

## 18B20 Temp

  ### * Codigo
  
  ### * Corrida
  
  ### * Imagenes del circuito

## Big Sound

  ### * Codigo
  
  ### * Corrida
  
  ### * Imagenes del circuito


## Touch

  ### * Codigo
  
  ### * Corrida
  
  ### * Imagenes del circuito
  
## Two-color

  ### * Codigo
  
  ### * Corrida
  
  ### * Imagenes del circuito
  
## Laser emit

  ### * Codigo
  
  ### * Corrida
  
  ### * Imagenes del circuito
 
## Laser emit

  ### * Codigo
  
  ### * Corrida
  
  ### * Imagenes del circuito
  
  
## Ball switch

  ### * Codigo
  
  ### * Corrida
  
  ### * Imagenes del circuito
  
## Analog temp

  ### * Codigo
  
  ### * Corrida
  
  ### * Imagenes del circuito

## Small sound
  
  ### * Codigo
  
  ### * Corrida
  
  ### * Imagenes del circuito

## Digital temperature

  ### * Codigo
  
  ### * Corrida
  
  ### * Imagenes del circuito

## Mini two-color

  ### * Codigo
  
  ### * Corrida
  
  ### * Imagenes del circuito
  
## Butom 

  ### * Codigo
  
  ### * Corrida
  
  ### * Imagenes del circuito
 
## Photo-esistor

  ### * Codigo
  
  ### * Corrida
  
  ### * Imagenes del circuito

## IR emission

  ### * Codigo
  
  ### * Corrida
  
  ### * Imagenes del circuito
  
## Tracking

  ### * Codigo
  
  ### * Corrida
  
  ### * Imagenes del circuito
  
## Buzzer

  ### * Codigo
  
  ### * Corrida
  
  ### * Imagenes del circuito
  
## Reed switch

  ### * Codigo
  
  ### * Corrida
  
  ### * Imagenes del circuito
  
## Shock

  ### * Codigo
  
  ### * Corrida
  
  ### * Imagenes del circuito
  
## Shock

  ### * Codigo
  
  ### * Corrida
  
  ### * Imagenes del circuito
  
## Ky-015 Temp 

  ### * Codigo
  
  ### * Corrida
  
  ### * Imagenes del circuito
  
## Ky-022 IR ???eiver 

  ### * Codigo
  
  ### * Corrida
  
  ### * Imagenes del circuito
  
## Avoidance 

  ### * Codigo
  
  ### * Corrida
  
  ### * Imagenes del circuito



    
