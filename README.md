# pico-pwm-audio
Raspberry Pi Pico PWM Audio Project

This code goes with a YouTube video (still to be published) which demonstrates PWM audio out with a simple cicruit on a raspberry pi pico. 

## Building

### Sync 
```
git clone git@github.com:rgrosset/pico-pwm-audio.git
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
