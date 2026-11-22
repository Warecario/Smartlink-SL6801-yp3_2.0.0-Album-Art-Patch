# Smartlink-SL6801-yp3_2.0.0-Album-Art-Patch:
A Album Art patch for mp3 players with chipset **Smartlink SL6801** running firmware **yp3_2.0.0** stock that shows the ablum/cover art of the mp3 in the Now Playing section.


### Supported Cover Art & Specs:

• Supported tags: **ID3v2.2** and **ID3v2.3 / ID3v2.4**, prioritizing the front cover.
• Image format: Baseline **JPEG** only.
• Display & scaling: Scales and center-crops the cover to fill the 128 by 160 display, dimming the brightness by 50% so the Now Playing text and UI overlays remain readable.

### Prerequisites:
Linux or Windows

https://github.com/ilyakurdyukov/smartlink_flash/

An mp3 player with a **SL6801** chip and **yp3_2.0.0 firmware.**

### Dump your firmware:
Linux:
```bash
sudo ./smtlink_dump init flash_id read_flash 0 2M stock_backup.bin
```

Windows:
```cmd
smtlink_dump.exe init flash_id read_flash 0 2M stock_backup.bin
```

### To patch:

**Note:
This is a full firmware binary, this replaces the firmware already on the player.**

Linux:
```bash
sudo ./smtlink_dump init write_flash 0 0 0 yp3_2.0.0_albumart.bin
```

Windows:
```cmd
smtlink_dump.exe init write_flash 0 0 0 yp3_2.0.0_albumart.bin
```

### What is this?
The stock **2.0.0 firmware** with a simple patch that shows the album/cover art of an mp3 in the Now Playing area.

### Tested:
Only tested on **yp3_2.0.0 firmware**, you can try to patch newer or older firmware, but they are not guarantee to work.

### Source Code:
If you would like the source code to fix any bugs that may appear when you flash it, please make an issue in the repo and I will get to it when I can.

### Credits:
I give credit where it is due, so huge thanks to **dbrant** at https://github.com/dbrant/SL6801_player for providing the main code used for this project.

Also a thanks to **zeroproj** at https://github.com/zeroproj/OpenPod for giving me the inspiration to do this project, and I am very glad it is finished.

Thanks to **ilyakurdyukov** at https://github.com/ilyakurdyukov/smartlink_flash/ for the tool.

Please go check out their work.
