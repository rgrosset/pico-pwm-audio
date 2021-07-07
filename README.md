# pico-pwm-audio
Raspberry Pi Pico PWM Audio Project

This code goes with a YouTube video which demonstrates PWM audio out with a simple cicruit on a raspberry pi pico. 

[![Raspberry Pi Pico Audio Output](https://img.youtube.com/vi/rwPTpMuvSXg/0.jpg)](https://www.youtube.com/watch?v=rwPTpMuvSXg)



## Building

### Sync 
```
git clone https://github.com/rgrosset/pico-pwm-audio.git
```

### Make 
Build project using cmake. This requires Raspberry Pi Pico C/C++ SDK to be installed. 
```
mkdir build
cd build
cmake ..
make
```

Then copy pico-pwm-audio.uf2 to your Raspberry Pi Pico!
