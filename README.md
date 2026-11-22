# Smartlink-SL6801-yp3_2.0.0-Album-Art-Patch
A Album Art patch for mp3 players with chipset Smartlink SL6801 running firmware yp3_2.0.0 stock that shows the ablum/cover art of the mp3 in the Now Playing section.

# To patch:

Note:
This is a full firmware binary, this replaces the firmware already on the player.

Linux:
sudo ./smtlink_dump init write_flash 0 0 0 yp3_2.0.0_albumart.bin

Windows:
smtlink_dump init write_flash 0 0 0 yp3_2.0.0_albumart.bin

# What is this?
The stock 2.0.0 firmware with a simple patch that shows the album/cover art of an mp3 in the Now Playing area.

# Tested:
Only tested on yp3_2.0.0 firmware, you can try to patch newer or older firmware, but they are not guarantee to work.

# Credits:
I give credit where it is due, so huge thanks to dbrant at https://github.com/dbrant/SL6801_player for providing the main code used for this project.

Also a thanks to zeroproj at https://github.com/zeroproj/OpenPod for giving me the inspiration to do this project, and I am very glad it is finished.

Please go check out their work.
