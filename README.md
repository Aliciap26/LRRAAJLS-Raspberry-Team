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
Codigo
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
utime.sleep(0.1) 
```

  ###  Corrida
  
  ###  Imagenes del circuito
  
  
 <a href="https://cooltext.com"><img src="https://images.cooltext.com/5626297.png" width="230" height="48" alt="RGB LED" /></a>
  Codigo
  
```
from machine import Pin
import time

led_pins = [16,17,18] # pins where RGB LED is wired
leds = [Pin(led_pins[0],Pin.OUT),Pin(led_pins[1],Pin.OUT),
        Pin(led_pins[2],Pin.OUT)] # pin control array
delay_t = 0.1 # seconds to delay between toggles
while True: # loop infinitely
    for led in leds: # loop through each led
        led.high() # led high
        time.sleep(delay_t) # wait
        led.low() # led low
        time.sleep(delay_t) # wait
 ```

  ### Corrida
  
  ###  Imagenes del circuito
  
  
<a href="https://cooltext.com"><img src="https://images.cooltext.com/5626301.png" width="258" height="78" alt=" Heartbeat" /></a>
  ###  Codigo
  
  ### Corrida
  
  ###  Imagenes del circuito
  
## Light cup
  ###  Codigo
  
  ###  Corrida
  
  ### * Imagenes del circuito

<a href="https://cooltext.com"><img src="https://images.cooltext.com/5626305.png" width="347" height="93" alt="Hall Magnetic" /></a>
  Codigo
 ```from machine import Pin
import utime

sensor=Pin(26, Pin.IN)
utime.sleep(1)

while True:
    if sensor.value()==1:
        print("Ningun campo detectado")
        utime.sleep(1)    
    else:
        print("Campo magnetico detectado")
        utime.sleep(1)
utime.sleep(1)
``` 
  ### * Corrida
  
  ### * Imagenes del circuito
  
 <a href="https://cooltext.com"><img src="https://images.cooltext.com/5626306.png" width="172" height="93" alt="Realy" /></a>

   Codigo
 ```
 from machine import Pin
import utime

relay = Pin(18,Pin.OUT)

while True:
    
    relay.value(1)
    utime.sleep(0.5)
    relay.value(0)
    utime.sleep(0.5)
```
  ### * Corrida
  
  ### * Imagenes del circuito
  
<a href="https://cooltext.com"><img src="https://images.cooltext.com/5626307.png" width="303" height="79" alt="Linear Hall" /></a>
  ### * Codigo
  
  ### * Corrida
  
  ### * Imagenes del circuito
  
<a href="https://cooltext.com"><img src="https://images.cooltext.com/5626308.png" width="244" height="49" alt=" SMD RGB" /></a>
 Codigo
```
from machine import Pin
import time

led_pins = [16,17,18] # pins where RGB LED is wired
leds = [Pin(led_pins[0],Pin.OUT),Pin(led_pins[1],Pin.OUT),
        Pin(led_pins[2],Pin.OUT)] # pin control array
delay_t = 0.1 # seconds to delay between toggles
while True: # loop infinitely
    for led in leds: # loop through each led
        led.high() # led high
        time.sleep(delay_t) # wait
        led.low() # led low
        time.sleep(delay_t) # wait
 ```

  ### * Corrida
  
  ### * Imagenes del circuito
  
<a href="https://cooltext.com"><img src="https://images.cooltext.com/5626309.png" width="280" height="79" alt="Color Flash" /></a>

Codigo

  
  ### * Corrida
  
  ### * Imagenes del circuito
  
<a href="https://cooltext.com"><img src="https://images.cooltext.com/5626310.png" width="261" height="79" alt="Tilt switch" /></a>

 Codigo
  
  ### * Corrida
  
  ### * Imagenes del circuito
  

<a href="https://cooltext.com"><img src="https://images.cooltext.com/5626312.png" width="295" height="90" alt="18B20 Temp" /></a>

Codigo
  
  ### * Corrida
  
  ### * Imagenes del circuito

<a href="https://cooltext.com"><img src="https://images.cooltext.com/5626313.png" width="295" height="90" alt="Big Sound" /></a>

Codigo
  
  ### * Corrida
  
  ### * Imagenes del circuito


<a href="https://cooltext.com"><img src="https://images.cooltext.com/5626314.png" width="149" height="73" alt="Touch" /></a>

  ### * Codigo
  
  ### * Corrida
  
  ### * Imagenes del circuito
  
<a href="https://cooltext.com"><img src="https://images.cooltext.com/5626315.png" width="225" height="72" alt="Two-color" /></a>

Codigo
 ```
from machine import Pin
import time

led_pins = [16,17] # pins where RGB LED is wired
leds = [Pin(led_pins[0],Pin.OUT),Pin(led_pins[1],Pin.OUT)] # pin control array
delay_t = 0.1 # seconds to delay between toggles
while True: # loop infinitely
    for led in leds: # loop through each led
        led.high() # led high
        time.sleep(delay_t) # wait
        led.low() # led low
        time.sleep(delay_t) # wait
 ```
  ### * Corrida
  
  ### * Imagenes del circuito
  


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



    
