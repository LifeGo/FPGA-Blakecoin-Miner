Icarus/Lancelot ports

LX150-Midstate         Original version, 16 clocks/hash, up to 16 cores
                       Best speed to date 89MHash/sec at 50MHz

LX150-Unrolled         Unrolled, 16 clocks/hash, 16 stages, up to 4 cores
                       Best speed to date 270MHash/sec at 45MHz (3 cores)

LX150-UnrolledPiped    32 clocks/hash, 32 stages, up to 4 cores
                       NB runs approx double clock speed due to extra pipelining
                       Best speed to date 450MHash/sec at 75MHz (3 cores)

LX150-MaxPiped         96 clocks/hash, 96 stages (6 latency G Function)
                       This is resource heavy, so FourPiped may be better.

LX150-FourPiped        64 clocks/hash, 64 stages (4 latency G Function)
                       Fast, perhaps 200MHz for a single core.

LX150-FourGatedClk     As above but using gated clock on the serial bus which may
                       route better. Work in progress.
					   
Any of the last three (or a variant) may give a good result, the difficulty is the
"random" nature of the Xilinx build process. LX150-FourGatedClk is the current
version, see ../bitstreams.txt for downloads and ../cgminer/cgminer-3.1.1 for
mining software (there is also a python miner in ../MiningSoftware, but this is
depreciated other than for test purposes).

X6500-Basic            Initial basic port to X6500. NOT WORKING, DO NOT USE.

X6500-Robust           Working version, see README in the folder.

CM1, DE0-Nano, Ztex 1.15x and Ztex 1.15y are detailed in their respective READMEs.