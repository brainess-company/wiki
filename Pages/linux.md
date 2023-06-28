# Linux
- How to set ABNT2 laoyut:

  `setxkbmap -model abnt2 -layout br -variant abnt2`
- How to change monitor outputs 

  `xrandr --output DVI-D-0 --primary --left-of HDMI-A-0`

- How install fonts: 
  - unpack the font archieve
  `$ tar -xzvf Hack-v3.003-ttf.tar.gz
   $ unzip JetBrainsMono.zip`

  - copy to your folder
  `/usr/share/fonts/
  ~/.local/share/fonts/
  /usr/local/share/fonts
  ~/.local/share/fonts/`

  - Clear and regenerate your font cache
  `$ fc-cache -f -v`

  - Virify the instalation
  `$ fc-list | grep "JetBrains"`
   
