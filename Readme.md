
## Aims
This repo is about to save the settings to make Wine works in Linux environment.

## Requirements
Linux OS, e.g Ubuntu  
Wine  
Winetricks  

## Install Wine and Winetricks in Ubuntu
```
sudo apt-get install winetricks
```

## Config the Display to zoom the GUI and fonts
    1. Open Winetricks  
    2. Selecte your wineprefix  
    3. Run winecfg -> Graphics -> Screen resolution -> 216 dpi  


## Install required dlls
```
# dlls required by WeChat input
winetricks dlls riched30  
winetricks dlls richtx32
winetricks apps firefox
```

## Config for Chinese fonts
1. Install the fonts
```
winetricks fonts wenquanyi  
```
2. Config the registry table  
    2.1 Open Winetricks  
    2.2 Selecte your wineprefix  
    2.3 Run Regedit  
    2.4 Import `configs/chn_fonts.reg`  
