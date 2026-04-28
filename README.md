# MegaDuck MD0 FlashCart

This FlashCart supports the MD0 Mapper by default.
To support the MD1 Mapper the Dioded D1 and D2 need to be removed (untested).

To support MD2 Mapper the flash needs to be altered:

As the banksize of MD2 is 16K and the Banksize of MD0 is 32K, bank0(MD0) is bank0+bank1(MD2)
bank1(MD0) is also bank0+bank1(MD2)
bank2(MD0) is bank0+bank2(MD2)
bank3(MD0) is bank0+bank3(MD2)
... etc


The binary needs to be altered to represent this scheme and should afterwards just work (also untested)

