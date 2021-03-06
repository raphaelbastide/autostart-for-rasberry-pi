# Auto startup files for rasberry pi
When rasberry pi boots, below applications automatically run

- homebase
- wiringPi
- chromium

clone all autostart files under /home/pi/

```terminal.app
pi@raspberrypi:~$ ls   
autostart_chromium.sh						 
autostart_homebase.sh						 
autostart.sh							 
autostart_sound.sh						  
```


## Auto start the fist terminal window
modify `~/.config/lxsession/LXDE-pi/autostart` following [this step1](https://www.raspberrypi-spy.co.uk/2014/05/how-to-autostart-apps-in-rasbian-lxde-desktop/)

```~/.config/lxsession/LXDE-pi/autostart
@lxpanel --profile LXDE-pi
@pcmanfm --desktop --profile LXDE-pi
# @xscreensaver -no-splash
# @point-rpi

@xset s off
@xset -dpms
@bash /home/pi/autostart.sh
```
# References
- [wiringPi](http://wiringpi.com/)
- [homebase](https://github.com/beakerbrowser/homebase)
- Vogelhaus documentation page dat://d0cdd1916150c0e9a6b6b1c66df16a2c5808c1135952d7bed925c4146eff7744/
