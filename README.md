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

## Using the Audito Converter Notebook. 

The conventer is a Jupyter Notebook so you need to install Jupyter Notebooks for this to work. These instructions will work on MacOS and Linux systems for Windows systems the proess is the same simply follow instructions to install Python and related items for that platform. 

### Installing 
* First you need a working install of Python preferably a 3.x verson. To install python if you don't have it already go here https://www.python.org/downloads/

* Second you need *pip* which is the python package manager, install this using the following
```
curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py
python get-pip.py
```

* Install the notebook dependancies. These are the python libraries the notebook needs to run. 
```
pip install soundfile 
pip install matplotlib
pip install samplerate
```


* Next you need to install Jupyter Notebooks you can find instructions and many ways to install here https://jupyter.org/install my favoured way to do this is simply
```
pip install notebook
```

* Then launch the notebook user interface by issueing this command in the same folder as this project. Open the notebook file in the user interface.  

```
jupyter notebook
```

The notebook itself is fairly self explanatory. Run each cell in order. The final cell will create a data array that you can copy and paste into your for your project. It will convert from WAV file to mono 11Khz data which you can then use in your projects! 


Have fun! Let me know if you have any feedback or questions. 
