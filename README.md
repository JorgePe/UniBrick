# UniBrick
A universal controller for LEGO devices

This gathers the several methods I use to control LEGO devices.

It started with the idea of a "Power Functions IR gateway" for a LUG fellow, as he can use
a computer keyboard much faster than myself but has troubles handling the LEGO Power Functions
remote controller. I gave him SSH access to a MINDSTORMS EV3 robot I had and he could control
it with his computer keyboard much like a computer game so I thought that he could do the same
with a LEGO Technic model if I give him a "Power Functions gateway".

So I started with a Raspberry Pi and a LIRC-compatible IR transmitter, mainly because:
- the RPi is powerfull and cheap (not as cheap as an Arduino but much more flexible to use)
- my previous experience with LIRC and ev3dev convinced me that LIRC can serve my needs of
portability and flexibility since I can use it on all my linuxes devices (EV3, RPi, x64 laptop)
and even with different transmitters and, in some cases, several transmitters at the same time.

For now I'll past to this repository all I got before with Infrared:
- Old LEGO RC protocol
- LEGO MINDSTORMS RCX IR command
- Power Functions IR

Later on I will add other non-Infrared technologies like:
- Interface A parallel port
- Interface B serial port
- MINDSTORMS VLL
- WeDo 2.0 BT BLE
- BOOST BT BLE
- Vengit SBrick (not LEGO) BT BLE
