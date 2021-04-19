# Pinnacle 100 Firmware Manifest Repo

## Using the Firmware

This firmware provides a template for using custom sensors with MG100. See more information [here](https://github.com/vascode/Pinnacle-100-Firmware/tree/custom_template)

## Cloning Firmware

This is a Zephyr `west` manifest repository. To learn more about `west` see [here](https://docs.zephyrproject.org/latest/guides/west/index.html).

To clone this repository properly use the `west` tool. To install `west` you will first need Python3.

Install `west` using `pip3`:

```
# Linux
pip3 install --user -U west

# macOS (Terminal) and Windows (cmd.exe)
pip3 install -U west
```

Once `west` is installed, clone this repository using `west init` and `west update`:

```
# Checkout the latest manifest on main
west init -m https://github.com/vascode/Pinnacle-100-Firmware-Manifest/tree/custom_template.git --manifest-rev main

# Now, pull all the source described in the manifest
west update
```

## Preparing to Build

If this is your first time working with a Zephyr project on your computer you should follow the [Zephyr getting started guide](https://docs.zephyrproject.org/latest/getting_started/index.html#) to install all the tools.

The firmware uses zephyr 2.4.x, so GCC 9 is recommended.
[GNU Arm Embedded Toolchain: 9-2020-q2-update](https://developer.arm.com/tools-and-software/open-source-software/developer-tools/gnu-toolchain/gnu-rm/downloads) is recommended.

See here to [setup the GNU ARM Embedded tools](https://docs.zephyrproject.org/2.4.0/getting_started/toolchain_3rd_party_x_compilers.html#gnu-arm-embedded)

If using Linux, v0.11.4 of the Zephyr SDK is recommended.

## Building the Firmware

See [here for build commands](https://github.com/vascode/Pinnacle-100-Firmware/blob/custom_template/docs/firmware_update.md#building-the-firmware).
