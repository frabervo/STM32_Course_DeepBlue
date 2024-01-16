# Getting Started with STM32 ARM Cortex MCUs

Goals: 
- introduction to STM32 ARM-Cortex based microcontrollers
- The internal architecture, buses and features
- discuss the reset and clock control circuitry with the clock tree

[Link for the tutorial 01](https://deepbluembedded.com/getting-started-with-stm32-arm-cortex-mcus/)

## STM32 ARM - Based Microcontrollers 

The development board selected for this series of tutorials: Nucleo-F446RE

Here is the core highlight diagramm for the STM32F446RE microcontroller part.

![core highlight](./pictures/stm32f446re.avif)

+ ARM Cortex-M4 Processor + FPU (Floating Point Unit)
Properties:
  - reduced pin count 
  - low-power consumption, while delivering outstanding computational performance and an advanced response to interrupts.

+ Adaptive Real-Time (ART) Accelerator: is a memory accelerator that is optimized for STM32 industry-standard Arm Cortex M4 processors.

  - It balances the inherent performance advantage of the ARM Cortex-M4 with FPU over Flash memory technologies, which normally requires the processor to wait for the Flash memory at higher operating frequencies. To release the processor full performance, the accelerator mplements an instruction prefetch queue and branch cache which increases program execution speed from the 128- bit Flash memory. Based on CoreMark benchmark, the performance achieved thanks to the ART accelerator is equivalent to 0 wait state program execution from Flash memory at a CPU frequency up to 180 MHz