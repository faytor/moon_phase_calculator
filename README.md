# Moon Phase Calculator

## Contents
***
- [General Info](#general-info)
- [Usage](#usage)
- [Test](#test)
- [References](#references)






## General Info
***
This is a simple algorithm to calculate Moon's Phase on a given date using the Arduino environment. Here, I used the [Heltec esp32 v2](https://heltec.org/project/wifi-lora-32/) development board.   
The algorithm is inspired by the magazine [skyandtelescope](https://skyandtelescope.org/wp-content/plugins/observing-tools/moonphase/moon.html).   
You can find also a previous version using an Arduino nano and a Nokia LCD display in my [old Github account](https://github.com/TorLab/MoonPhaseCalculation).

## Usage
***
The main function is moonPhases(int year, int month, int day) where 'year' is a four-digit number.
```
/* Calculate the moon number */
moonNum = moonPhases(year, month, day);
```
Where ``moonNum`` corresponds to the "moon day/age", as well as the bitmap image to be drawn on the OLED display.   
A Time zone is also needen in the calculation of the Julian day : 
```
int timeZone = 2;
```

Inputs example:

```
int timeZone = 2;
int day = 8;
int month = 8;
int year = 2021;
```


## Test
***
Make sure to install the fellowing dependencies to test the program:
* [u8g2 Library](https://github.com/olikraus/u8g2/wiki)   





## References
***

- [U8g2 Font List](https://github.com/olikraus/u8g2/wiki/fntlist8#5-pixel-height)
- [Sky & Telescope](https://skyandtelescope.org/wp-content/plugins/observing-tools/moonphase/moon.html)
