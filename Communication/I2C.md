Flow of Communication:

1. Central device sends start bit
2. Central device sends 7-bit slave address of the peripheral device it wants to "talk" to
3. Central device sends either read or write
4. Peripheral device acknowledges request (logic low)
5. a) Write Mode: Central device sends 1 byte at a time, peripheral acknowledges (logic low)
   b) Read Mode: Master device receives 1 byte at a time & sends acknowledgement bit to peripheral device after each byte
6. When communication is complete, the master device sends a stop bit
