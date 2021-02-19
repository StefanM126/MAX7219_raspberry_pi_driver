# MAX7219_raspberry_pi_driver
Driver for one or four rpi matrixes, depending on insmod parameters.

Building with 'make'
Starting driver with 'sudo insmod gpiod_driover.ko  Res="res" AlwaysInit="alwI" '

res - resolution is defined by string formated like: "numxnum", suported resolutions are 1x1 and 2x2 (default 1x1)
alwI - on by default, can be turned of with: AlwaysInit="off"; Only exists due to problem with quick power loss after which the controller is uninitialized.
