# STM32F1 USB Project template

This is a template project for any STM32F1 microcontroller using the USB middleware provided by ST. In order to select the appropiate microcontroller model, you need to:

* Change the $(CPU) alias in the Makefile to match your MCU.
* Change the $(LDSCRIPT) alias in Makefile to match your corresponding MCU. LD scripts are located in cmsis/linker/
* Change -D option in CFLAGS to match your MCU.
* Change the startup_stm32f1**.s accordingly. They are located in cmsis/device/src/

The default project is for a CDC device. If you wish to change the device class, replace the files in the usb_class folder with the ones found in USB_CLASSES.
