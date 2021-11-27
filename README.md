# SKR-mini-E3-V3.0-Beta-STM32G0B1RET6
SKR-mini-E3-V3.0 built on the latest version of Marlin Debug.

Loaded everything from the BigTreeTech STM32G0B1RET6 repository into the latest version of Marlin bugfix - 2.0.x. 

This fixes the no cooling fan and controller fan issue. 

Double check the FACONTROLLER_FAN_PIN located in Marlin\src\pins\stm32g0\pins_BTT_SKR_MINI_E3_V3_0.h for this board. It might be assisted to the wrong fan pin and I will address this in a future release. (please let me know)

# Important Note From BigTreeTech
* Please copy the 4 files `variant_MARLIN_STM32G0B1RE.cpp`, `variant_MARLIN_STM32G0B1RE.h`, `ldscript.ld`, `PeripheralPins.c` in the path [buildroot/share/PlatformIO/variants](https://github.com/bigtreetech/Marlin-Pri/tree/SKR-mini-E3-V3.0/buildroot/share/PlatformIO/variants) to the path of STM32Duino dependent library in your computer `C:\Users\Administrator\.platformio\packages\framework-arduinoststm32\variants\STM32G0xx\G0B1R(B-C-E)(I-T)xN_G0C1R(C-E)(I-T)xN`
Otherwise, the compiler will report an error or missing file!
