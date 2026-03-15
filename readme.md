# TOTEM ZMK Config

This repository contains my ZMK configuration for the TOTEM split keyboard.

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="/docs/images/TOTEM_logo_dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="/docs/images/TOTEM_logo_bright.svg">
  <img alt="TOTEM logo font" src="/docs/images/TOTEM_logo_bright.svg">
</picture>

TOTEM is a 38-key column-staggered split keyboard that runs [ZMK](https://zmk.dev/) or [QMK](https://docs.qmk.fm/). It is designed for the SEEED XIAO BLE or RP2040.

![TOTEM layout](/docs/images/TOTEM_layout.svg)

<img width="911" height="1518" alt="TOTEM keymap preview" src="https://github.com/user-attachments/assets/cf64ad49-f5ff-4a50-a76b-4ff352f98e3f" />

## Flashing Firmware

1. Download the firmware from the GitHub Actions tab.
2. Keep both halves powered on.
3. Plug in the left half and press the reset button twice quickly. A storage drive should open on your computer.
4. Drag and drop the settings reset file onto the left half.
5. Unplug the left half, plug in the right half, and press reset twice quickly. A storage drive should open on your computer.
6. Drag and drop the settings reset file onto the right half.
7. Unplug the right half and plug the left half back in.
8. Press reset twice.
9. Drag and drop the left firmware file onto the left half.
10. Unplug the left half and plug in the right half.
11. Press reset twice.
12. Drag and drop the right firmware file onto the right half.

## How To Use

1. Clone this repository to your computer.
2. Update `config/totem.keymap` with your preferred layout. Keycode references are available in the [ZMK docs](https://zmk.dev/docs/codes/).
3. Push your changes to your GitHub repository.
4. Open the repository on GitHub and go to the `Actions` tab.
5. Download and unzip the latest `firmware.zip` build artifact.
6. Connect the left half of the TOTEM to your computer and press reset twice.
7. Wait for the keyboard to appear as a mass storage device.
8. Drag and drop `totem_left-seeeduino_xiao_ble-zmk.uf2` onto the device.
9. Repeat the same process with the right half using `totem_right-seeeduino_xiao_ble-zmk.uf2`.
