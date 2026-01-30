# ASUS UM5606 Firmware Update Checker
Dead-simple bash script to check if the UM5606 laptop has a BIOS update

## Models supported
- UM5606WA (tested)
- UM5606KA
- UM5606GA

## Dependencies
- bash
- curl
- coreutils
- notify-send (optional)

## Installation
- Arch Linux: `yay -S asus-5606-firmware-check-git`
- All others: copy `asus_firmware_check` to anywhere in `$PATH`

## Usage
Just run `asus_firmware_check`. If there's an update, it'll tell you. If not, it'll exit with 0.

I personally run this in a systemd user service with a timer that fires every Monday.
