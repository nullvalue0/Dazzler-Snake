# DazzlerSnake
 Dazzler Snake game for the Cromemco Dazzler

This is a new game developed for the Cromemco Dazzler video card. It was developed in Z80 Assembly, directly on real hardward including an original Cromemco ZPU, D+7A, Memory Merchant 64KB RAM, and a [reproduction dazzler board set](https://forum.vcfed.org/index.php?threads/cromemco-dazzler-replica-project.77906/). These are all plugged into the S100 Motherboard V5(https://github.com/nullvalue0/S100MotherboardV5). Game was sssembled using the original Cromemco Z80 Macro Assembler.

![Snake running on real hardware](https://github.com/nullvalue0/Dazzler-Snake/blob/main/snake_hardware.jpg?raw=true)

This game borrows some of the graphics routines from the GDEMO application, which in turns uses the GRAPHZ80 library. This was original software library distributed with the Dazzler and simplifies things like pixel addressing, drawing lines and selecting colors.

This game can take input from a keyboard or joystick. For joystick, I am using a pair of [replica JS-1 joysticks](https://forum.vcfed.org/index.php?threads/cromemco-js-1-joystick-replica.1247727/). The joystick inputs get read in through a D+7A card using the default port configuration. The game also features sound, as the joysticks each provide a speaker. The code for joystick input & sound I borrowed from the "GOTCHA" game originally distributed with the Dazzler.

![Snake running emulated in z80pack](https://github.com/nullvalue0/Dazzler-Snake/blob/main/snake_emulator.png?raw=true)

This is the first application I have ever written in Z80 ASM, and has been a very rewarding experience. The code is extremely unoptimized, but it works!!