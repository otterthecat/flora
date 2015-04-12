#BagLite
Light up the inside of your bag.

## How It Works
Using the Adafruit [Lux Sensor](https://learn.adafruit.com/flora-lux-sensor) combined with conductive velcro to act as a swtich,
if the sensor determines it is dark outside, AND if the velcro swith is "on" (which, in our case, means pulled apart),
that will tell the Flora to turn on the [NeoPixel](https://learn.adafruit.com/flora-rgb-smart-pixels?view=all) lights so you can see the inside of your bag.

Project inspired by [Interior Light Purse](https://learn.adafruit.com/interior-purse-light?view=all)

## Pin Setup

### Lux Sensor
Flora 3.3v -> Lux 3v
Flora SDA -> Lux SDP
Flora SCL -> Lux SCL
Flora GND(next to usb input) -> Lux GND

### NeoPixel(s)
Flora VBATT -> NeoPixel (+)
Flora D6 -> NeoPixel IN (arrow pointing to center)
Flora GND -> NeoPixel (-)

### Pull-Up (Velcro) Switch
Flora D10 -> Soft Side Velcro
Flora GND (shared with NeoPixel) -> Hook Side Velcro
