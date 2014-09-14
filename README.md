HostTestApp-SensorTag
=====================

HostTestApp (HCI) implementation for TI SensorTag board

You actually need Projects/ble/HostTestApp, all the other stuff is kept in order to preserve directory structure.

Modifications:

  1. HAL files are changed to use **UART0, Alt.2** instead of **UART0 Alt.1** (SensorTag has UART0 Alt.2 pins wired to side pads),
  2. During power up, "Start\r\n" string is send to UART,
  3. Hardware **flow control is disabled**
