fix-airplay
===========

A simple script that kills the coreaudio daemon to fix common AirPlay problems. I wrote a little [blog post](http://benlimmer.com/2013/12/30/airplay-not-working-try-this/) about why I needed this.

# Download
Get the application [here](https://github.com/l1m5/fix-airplay/raw/master/FixAirplay.app.zip).

# Script
You can also just run this from the terminal:
```bash
sudo kill `ps -ax | grep 'coreaudiod' | grep 'sbin' |awk '{print $1}'`
```
