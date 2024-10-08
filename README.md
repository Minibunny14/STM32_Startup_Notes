# 
This is a repository of knowledge surrounding the STM32 microcontroller.

# STM32
## What is an STM32:
The STM32 is a variant of the 32-bit microcontroller's that are based on the ARM Cortex-M architecture(more about this on another section). 
STM32 is a popular board choice in embedded systems applications, due to their high performace, power efficiency and widr range of features.
The STM32 series is divided isnt multible sub-branches, each targeting different application requirements.

## Features:
1. STM32 boards are based on the ARM Cortex-M processor.
2. Peripherals: They offer various built-in peripherals such as ADC's, DAC's, timers, communication interfaces such as (UART, SPI, I2C, CAN) etc.
3. Development enviroment: STMicroelectronics provides a decent development environment, including IDE's such as STM32CubeIDE, firmware libraries.

# Nucleo Board
The Nucleo board is a development board series that is created by STMicroelectronics that uses the STM32 as its microcontroller. There are various NUCLEO boards available such as the NUCLEO-F0, NUCLEO-F3 and the NUCLEO-F4. 
- ## NUCLEO-F0:
    1. 
- ## NUCLEO-F3:
    1. 
- ## NUCLEO-F4:
    1.  

# BackGround(To understand the operation and application of the STM32)

## Communication Interfaces
The STM32 utilises communication interfaces described earlier, such as UART, I2C, SPI and CAN. Communication interfaces are the different mechanisms that two or more devices use to exchange information and interact with each other, in this case, how a microcontroller and a peripheral device(a) can be connected.

### SPI: Serial Peripheral Interface
SPI also known as the 


![Alt text](./Images/SPI_INTERFACE_LEADING_EDGE.drawio.png)

## ARM Cortex-M

### Purpose and Design:
* The Cortex-M series was build to be cost-sensitive, energy-efficient for embedded applications.
* It is mainly tuned to be used for microcontrollers such as the STM32

### Features:
* Cortex-M cores use a 32-bit RISC(Reduce Instruction Set Computing) architectrure. This essentially simplifies the design of the processors and makes its execution more efficient.
* Low Power Consumption
* Cortex-M processors come with built-in debugging features, this includes hardware breakpoints etc.

### Cortex-M Series Varients:
The STM32 has different neucleo boards, this includes the F-0 and F-4 series, the main difference is that the F-0(STM32F0) uses the ARM Cortex-M0 processor and the F-4(STM32F4) uses the ARM Cortex-M4 processor.

#### Cortex-M0
* This would be the simplest and smallest of the Cortex-M series, which is ideal for basic control tasks
#### Cortex-M3
* Optimisation done to provide a balance between performace and power effeciency, its often used in more complex embedded applications.
#### Cortex-M4
* Here is where Digital Signal Processing (DSP) instructions is added, which is useful for audio processing(signal sampling etc.), motor control and more. Essentially this would be used mainly for robotics, mechatronics etc.



### Registers and Memory:
Like most processors, the Cortex-M processors have a simple register structure, with 16 registers(including general purpose registers (R0-R12)). The Link Register(LR), the Program Counter(Counter) and a Stack Pointer(SP). Registers are storage locations that hold data or memory addresses.
#### Link Register:
The link register is used for holding the return address when calling a function or subroutine(Assembly).
#### Program Counter: 
The Program Counter is used to track the memory address of the next intruction to be executed in a program. Essentially, this could be thought of as the different steps in a recipe.
#### Stack Pointer:

The Stack Pointer is used to store the memory address of the last data element added to the stack or, the first available address in the stack.
