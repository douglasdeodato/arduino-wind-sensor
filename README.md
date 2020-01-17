# arduino-wind-sensor

from: https://www.qsl.net/on7eq/projects/arduino_davis.htm

ARDUINO readout of DAVIS Wind Sensor
This sketch will readout a DAVIS Wind sensor (Vantage Pro & Vantage Pro 2) and display the wind direction & speed on a 2x 16 character LCD display. The same low cost wind sensor is available from other sources (see specs here)




In addition, the temperature is measured with a 10k NTC resistor, which can be mounted outside, close to the wind sensor.

The wind vane direction can be permanently calibrated with following procedure : upon startup of the ARDUINO board, depress the CAL button while the vane is oriented towards the true North.  From that moment on, the correction is stored in EEPROM and readouts will be correct.




This is the sketch  or download it here.   It was compiled with IDE version 0022.- IMPORTANT : please use the same or you might get errors when compiling !  You still can download previous versions from ARDUINO website . The interrupt is triggered by FALLING level, because RISING proved to be less accurate at high wind speed.  The code called by the interrupt provides a timer (15 ms) to avoid REED contact bounce, it will allow to measure wind speeds in excess of 150 km/h.


another project:

https://www.geeky-gadgets.com/arduino-wind-speed-meter-anemometer-project-30032016/

– Adafruit Anemometer (product ref: 1733) – £39 or $44
https://www.amazon.co.uk/gp/product/B00PLVJDF6/ref=ox_sc_act_title_1?smid=A3VZWH9QVI2V2M&psc=1
– Arduino Uno or similar such as the new Arduino 101 or Genuino – £28 or $40 (cheaper clones are available)
https://www.amazon.co.uk/Intel-ATLASEDGE-2-Genuino-Computiong-Devices/dp/B0198HHSSM/ref=sr_1_2?keywords=Arduino+101&qid=1579260820&s=electronics&sr=1-2
– Arduino 16×2 LCD screen with keypad £2.50 or $3.60
https://www.amazon.co.uk/DOLITY-Screen-Expansion-Display-Arduino/dp/B07DL7FC6L/ref=sr_1_3?keywords=Arduino+16%C3%972+LCD+screen+with+keypad&qid=1579260841&s=electronics&sr=1-3
– 15m of 3 core cable – £10 or $14
– 12v Mains Power Supply £5 – $7
– Arduino IDE software loaded on to a PC or Mac – Free
https://www.arduino.cc/en/main/software
