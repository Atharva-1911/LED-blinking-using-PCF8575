START

Initialize serial communication with baud rate 115200

Create PCF8575 object with I2C address 0x20

BEGIN SETUP
    Set pin P0 of PCF8575 as OUTPUT
    Initialize PCF8575 I2C communication
END SETUP

BEGIN LOOP
    Set P0 output to LOW      // Turn LED ON (active LOW)
    Wait for 500 milliseconds

    Set P0 output to HIGH     // Turn LED OFF
    Wait for 500 milliseconds
END LOOP

END
