#####################
# Manta M8P Klipper #
#####################
[*] Enable extra low-level configuration options\
    Micro-controller Architecture (STMicroelectronics STM32) --->\
    Processor model (STM32H723) --->\
    Bootloader offset (128KiB bootloader (SKR SE BX v2.0)) --->\
    Clock Reference (25 MHz crystal) --->\
    Communication interface (USB to CAN bus bridge (USB on PA11/PA12)) --->
    CAN bus interface (CAN bus (on PD0/PD1)) --->
    USB ids --->
(1000000) CAN bus speed
() GPIO pins to set at micro-controller startup

######################
# Manta M8P Katapult #
######################
    Micro-controller Architecture (STMicroelectronics STM32) --->
    Processor model (STM32H723) 
    Build Katapult deployment application (128KiB bootloader (SKR SE BX v2.0)) ---> 
    Clock Reference (25 MHz crystal) ---> 
    Communication interface (USB (on A11/PA12)) ---> Application start offset (128KiB offset) USB ids ---> () GPIO pins to set on bootloader entry
[*] Support bootloader entry on rapid double click of reset button 
[] Enable bootloader entry on button (or gpio) state 
[] Enable Status LED

###################################
# BTT EBB SB2209v(RP2040) Klipper #
###################################
[*] Enable extra low-level configuration options
    Micro-controller Architecture (Raspberry Pi RP2040) --->
    Bootloader offset (16KiB bootloader) --->
    Communication interface (CAN bus) --->
(4) CAN RX gpio number (NEW)
(5) CAN TX gpio number (NEW)
(1000000) CAN bus speed
(gpio26) GPIO pins to set at micro-controller startup

###################################
# BTT EBB SB2209v(RP2040) Katapult #
###################################
    Micro-controller Architecture (Raspberry Pi RP2040) --->
    Flash chip (W25Q080 with CLKDIV 2) --->
    Build Katapult deployment application (16KiB bootloader) --->
    Communication interface (CAN bus) --->
(4) CAN RX gpio number (NEW)
(5) CAN TX gpio number (NEW)
(1000000) CAN bus speed
() GPIO pins to set on bootloader entry
[*] Support bootloader entry on rapid double click of reset button
[] Enable bootloader entry on button (or gpio) state
[*] Enable Status LED
(gpio26) Status LED GPIO Pin
