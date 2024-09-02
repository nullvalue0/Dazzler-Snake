# Dazzler Snake
 Dazzler Snake game for the Cromemco Dazzler

This is a new game developed for the Cromemco Dazzler video card. It was written in Z80 Assembly on real hardward including an original Cromemco ZPU, D+7A, Memory Merchant 64KB RAM, and a [reproduction dazzler board set](https://forum.vcfed.org/index.php?threads/cromemco-dazzler-replica-project.77906/). These cards are all plugged into a [S100 Motherboard V5](https://github.com/nullvalue0/S100MotherboardV5). Game was assembled using the original Cromemco Z80 Macro Assembler.

*Snake running on real hardware*
![Snake running on real hardware](https://github.com/nullvalue0/Dazzler-Snake/blob/main/snake_hardware.jpg?raw=true)

I referenced the GDEMO application source for how to use the graphics routines, which in turns uses the GRAPHZ80 library. This was the original software library distributed with the Dazzler and simplifies things like pixel addressing, drawing lines and selecting colors.

The game can be played in one or two player mode. It can take input from either the keyboard or joysticks. I am using a pair of [replica JS-1 joysticks](https://forum.vcfed.org/index.php?threads/cromemco-js-1-joystick-replica.1247727/). The joystick inputs get read in through a D+7A card using the default port configuration. The game also features sound, as the JS-1 each provide a speaker. The code for joystick input & sound I borrowed from the "GOTCHA" game originally distributed with the Dazzler.

*Snake running emulated in z80pack*
![Snake running emulated in z80pack](https://github.com/nullvalue0/Dazzler-Snake/blob/main/snake_emulator.png?raw=true)

This is the first application I have ever written in Z80 ASM, and has been a very rewarding experience. The code is extremely unoptimized, but it works! Special thanks for all the help to the folks at the VCF Forum!

With version 1.1, I've added CP/M support. Run SNAKE.COM for CDOS, or SNAKECPM.COM under CP/M.