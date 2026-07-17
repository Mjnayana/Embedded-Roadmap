# Embedded Firmware Roadmap - Zero to Interview-Ready

Tracking my transition from Hardware Engineer (3 yrs) into Embedded Software/Firmware,
following a 35-day, 5-week plan (2-3 hrs weekdays, 5-6 hrs weekends).
Board: STM32 Nucleo.

Source plan: `docs/Embedded_Firmware_Roadmap_ZeroToHero.pdf` (add your copy here)

## Progress Tracker

| Week | Focus | Status |
|------|-------|--------|
| 1 | Absolute C fundamentals | [ ] Not started |
| 2 | Embedded C habits, toolchain, memory/linker, bare-metal GPIO | [ ] Not started |
| 3 | UART, timers/PWM, interrupts | [ ] Not started |
| 4 | SPI, I2C, ADC, DMA, real debugging tools | [ ] Not started |
| 5 | Drivers, RTOS, portfolio project, interview prep | [ ] Not started |

Update status per week: Not started -> In progress -> Done

## Daily Log

Each `dayNN/` folder has its own `README.md` with: topics, what I built, code, and a one-line
"why I made this design choice" note.

| Day | Topic | Link |
|-----|-------|------|
| 1 | Set up and write your first program | [day01](week1_c_fundamentals/day01) |
| 2 | Variables, data types, and operators | [day02](week1_c_fundamentals/day02) |
| 3 | Conditionals and loops | [day03](week1_c_fundamentals/day03) |
| 4 | Functions and arrays | [day04](week1_c_fundamentals/day04) |
| 5 | Strings and a first taste of memory | [day05](week1_c_fundamentals/day05) |
| 6 | Pointers, part 1 | [day06](week1_c_fundamentals/day06) |
| 7 | Pointers, part 2 + structs | [day07](week1_c_fundamentals/day07) |
| 8 | Bit manipulation | [day08](week2_embedded_c_and_first_hardware/day08) |
| 9 | Function pointers, volatile, static, const | [day09](week2_embedded_c_and_first_hardware/day09) |
| 10 | Fixed-width types and unions | [day10](week2_embedded_c_and_first_hardware/day10) |
| 11 | Toolchain setup | [day11](week2_embedded_c_and_first_hardware/day11) |
| 12 | How a program gets onto a chip | [day12](week2_embedded_c_and_first_hardware/day12) |
| 13 | Memory map and linker scripts | [day13](week2_embedded_c_and_first_hardware/day13) |
| 14 | Bare-metal GPIO | [day14](week2_embedded_c_and_first_hardware/day14) |
| 15 | UART, part 1 (polling) | [day15](week3_comm_timing_interrupts/day15) |
| 16 | UART, part 2 + ring buffers | [day16](week3_comm_timing_interrupts/day16) |
| 17 | Timers | [day17](week3_comm_timing_interrupts/day17) |
| 18 | PWM | [day18](week3_comm_timing_interrupts/day18) |
| 19 | Interrupts, theory | [day19](week3_comm_timing_interrupts/day19) |
| 20 | Interrupt-driven UART | [day20](week3_comm_timing_interrupts/day20) |
| 21 | Interrupt-driven button + traffic light | [day21](week3_comm_timing_interrupts/day21) |
| 22 | SPI | [day22](week4_spi_i2c_adc_dma_debug/day22) |
| 23 | I2C | [day23](week4_spi_i2c_adc_dma_debug/day23) |
| 24 | ADC | [day24](week4_spi_i2c_adc_dma_debug/day24) |
| 25 | DMA | [day25](week4_spi_i2c_adc_dma_debug/day25) |
| 26 | Real debugging with GDB and OpenOCD | [day26](week4_spi_i2c_adc_dma_debug/day26) |
| 27 | Using hardware background as a firmware tool | [day27](week4_spi_i2c_adc_dma_debug/day27) |
| 28 | Watchdog + low-power modes | [day28](week4_spi_i2c_adc_dma_debug/day28) |
| 29 | Layered driver design | [day29](week5_drivers_rtos_portfolio/day29) |
| 30 | Makefiles | [day30](week5_drivers_rtos_portfolio/day30) |
| 31 | RTOS concepts and your first task | [day31](week5_drivers_rtos_portfolio/day31) |
| 32 | RTOS synchronization | [day32](week5_drivers_rtos_portfolio/day32) |
| 33 | RTOS queues and interrupts together | [day33](week5_drivers_rtos_portfolio/day33) |
| 34 | Build your portfolio project | [day34](week5_drivers_rtos_portfolio/day34) |
| 35 | Finish, document, and rehearse | [day35](week5_drivers_rtos_portfolio/day35) |

## Portfolio Project

The capstone (Days 34-35): a multi-sensor RTOS data-acquisition system in FreeRTOS -
sensor task (I2C/SPI) feeds a queue, logger task (UART) drains it, button-interrupt
semaphore switches modes, shared resources protected by a mutex.
See `portfolio-project/`.

## Boards / Tools

- STM32 Nucleo (primary), Blue Pill (secondary bare-metal practice)
- arm-none-eabi-gcc, OpenOCD + arm-none-eabi-gdb, make, FreeRTOS

## Glossary

Running list of new terms - see `notes/glossary.md`.
