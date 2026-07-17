# Portfolio Project - Multi-Sensor RTOS Data-Acquisition System

Capstone (Days 34-35). FreeRTOS app on STM32 Nucleo:

- Sensor task: samples I2C/SPI, feeds a queue
- Logger task: drains queue, logs over UART
- Mode task: switches modes on button-interrupt semaphore
- Shared resources protected by a mutex

## Build
```
make
make flash
```
