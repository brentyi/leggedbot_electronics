# Sparky electrical

![boards](/Project%20Outputs%20for%20LeggedBot/board.png)

Repository for the primary control PCB of our hexapedal robot.

Features:
- three TB6612 dual h-bridge driver ICs controlled through a PCA9685 PWM driver (for running 6 individual leg motors)
- an ADXL345 3-axis accelerometer for orientation detection
- an MP1584 5V/3A buck converter (primarily to make powering external devices easy)
- an N-fet-based electronic power switch
- three I2C output connectors for our absolute encoders - these were daisy chained, so we really only needed one
- a filtered battery voltage measurement input

To cut costs and reduce complexity, the board is designed to plug into an ATmega328P-powered Arduino Nano microcontroller.

---

[Demo video](https://www.youtube.com/watch?v=aiBIEI0JHwY) and relevant repositories:
- [firmware](https://github.com/brentyi/sparky_firmware)
- [mechanical design](https://github.com/nanditapiyer/sparky_mechanical)
- [absolute encoder PCB](https://github.com/brentyi/as5048b_breakout)
