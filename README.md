<p align="center"><img src="extra/kunst_logo.png"><br><sub>✨ Display embedded album art for mpd tracks ✨</sub></p>

```kunst``` is a deamon that extracts the album art from the songs playing in ```mpd``` and displays them in the a little window. It doesn't loop on a timer, instead it waits for ```mpd``` to send a ```player``` event. When it receives a ```player``` event, it wakes up and extracts the album art of the current playing track. This maks ```kunst```really lightweight and makes it idle at ```~0%``` CPU usage. 
 

**Note:** ```kunst``` is meant to be used with files that have embedded album art. But, if a song that is currently playing, does not have an embedded album art, an image of a music note will be shown.

<p align="left">
<img src="extra/demo.gif" width="657.8" height="438.1">
</a>
</p>

## Dependencies
- ```sxiv```
- ```imagemagick```
- ```bash```
- ```ffmpeg```
- ```mpc```

## Installation
Add ```kunst``` to a directory which is in you ```$PATH```

**OR**

[AUR](https://aur.archlinux.org/packages/kunst-git/)

## TODO

- [x] use less CPU
- [ ] add arguments (need to learn how to do this)
  - [x] music directory
  - [x] image size (dimentions)

## License
MIT License

Copyright © 2019 Siddharth Dushantha
