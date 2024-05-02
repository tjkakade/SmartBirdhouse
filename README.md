# SmartBirdhouse
ECE 4180 Final Project

![]((https://github.com/tjkakade/SmartBirdhouse/blob/main/images/house1.jpg))


## Parts List

### Electronics:

- **1 Mbed LPC1768**: [Available here](https://www.sparkfun.com/products/9564)
- **VL53L0X ToF Sensor**: [Available on Amazon](https://www.amazon.com/ARCELI-Sensor-Droplet-Detection-Arduino/dp/B07BP7B9TR)
- **ICM-20948 IMU**: [Available here](https://www.sparkfun.com/products/13322)
- **1 DC Motor**: [Available here](https://www.sparkfun.com/products/8688)
- **RaspberryPi Zero W**: [Available here](https://www.sparkfun.com/products/8688)
- **RaspberryPi Camera**: link_goes_here

### Non-electronics:

- A Birdhouse

## Pin Connection Guide

| LPC1768 Pin | Component | Component Pin | Other Pin |
|-------------|-----------|---------------|-----------|
| p9          | ICM20948  | DA            | -         |
| p10         | ICM20948  | CL            | -         |
| Vout (3.3V) | ICM20948  | Vin           | -         |
| GND         | ICM20948  | ADO           | -         |
| GND         | ICM20948  | GND           | -         |
| Vout (3.3V) | VL53LOX   | Vin           | -         |
| GND         | VL53LOX   | GND           | -         |
| p28         | VL53LOX   | SDA           | -         |
| p27         | VL53LOX   | SCL           | -         |
| p26         | VL53LOX   | SHDN          | -         |
| -           | TB6612FNG | AIN1          | Motor Lead (R) |
| -           | TB6612FNG | AIN2          | Motor Lead (B) |
| -           | TB6612FNG | VMOT          | Motor Power + |
| Vout (3.3V) | TB6612FNG | STBY          | -         |
| GND         | TB6612FNG | GND           | -         |
