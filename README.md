# Keyboard
model: ymdk/ymd40

## Install and configure qmk software

Install the qmk software for flashing by running: 

`yay qmk` or `sudo pacman -S qmk`.

Configure the default directory for flashing and default keyboard type by running:

`qmk setup`

Setup the default kb (keyboard) and default km (keymap)

## Create a keymap json file

Create or edit your keymap json file at [qmk configurator](https://config.qmk.fm/#/ymdk/ymd40/air40/LAYOUT_ortho_4x12_1x2uC)

Download your keymap.json file.

## Compile the firmware

Compile the firmware from the keymap.json file with

`qmk json2c -o ~/qmk_firmware/keyboards/ymdk/ymd40/air40/keymaps/{your_default_keymap_folder}/keymap.c ./keymap.json`

## Put your keyboard into a bootloader mode

To reset the board into bootloader mode, hold the key at the top left of the keyboard while connecting the USB cable (also erases persistent settings).

## Flash

Flash your default keymap to your default keyboard with:

`qmk flash`

