# corne-kb-firmware
Default firmware for the corne split keyboard.

prerequisites:
QMK toolbox is installed
https://github.com/qmk/qmk_toolbox

1. download crkb_rev1_default.hex
2. open QMK Toolbox and open the firmware file
3. connect the slave half (right hand) for the corne keyboard
4. reset the slave side
5. flash the firmware
6. connect the master half (left hand) for the corne keyboard
7. reset the master side
8. flash teh firmware
9. Test the keyboard is working as intended

**NOTE:** While doing this I had the trs/trrs plugged in while flashing both sides. If you flash the slave side second you may notice your keyboard is backwards. Just reflash the master side and it should sort it.

## OR
Build your own firmware

prerequisites:
QMK toolbox is installed
https://github.com/qmk/qmk_toolbox
QMK MSYS is installed
https://msys.qmk.fm/

Windows:
1. setup the QMK environment https://docs.qmk.fm/#/newbs_getting_started
2. copy the crkbd folder to qmk_firmware/keyboards (this will probably be in your user folder c:\username\qmk_firmware)
3. replace/overwrite the files if prompted.
4. make any changes you want, layout is default
5. open QMK MSYS
6. build the firmware with qmk compile -kb crkbd -km default
7. if all goes well the firmware will be in the root of the qmk_firmware folder
8. follow steps 2 - 9 above to flash.


