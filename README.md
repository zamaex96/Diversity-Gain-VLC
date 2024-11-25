Implementation of diversity gain combining techniques such as equal gain combining (EGC), majority logic combining (MLC), and delection combining (SC) on stm32 platform.

# Summary of `main.c`

## Overview

The `main.c` file serves as the main program body for an STM32 microcontroller-based application. It integrates functionalities for analog-to-digital conversion (ADC), UART communication, and signal processing techniques.

## Key Features

- **Initialization and Configuration**:
  - Configures system clock, GPIO, ADC, DMA, and UART peripherals.
  
- **ADC Configuration**:
  - Reads three differential channels using DMA for continuous data acquisition.
  
- **UART Communication**:
  - Initializes UART1 for bidirectional data transfer at 115200 baud rate.
  
- **Signal Processing**:
  - **DiversityGainEngineInit**: Manages ADC conversions, calculates threshold voltages, and selects combining techniques.
  - **ThresholdVoltageEstimator**: Determines maximum voltage among three inputs.
  - **CombiningTEchniqueSelection**: Implements logic for selecting combining techniques (EGC, MLC, SC) based on acquired voltages.
  - **EGC_Engine, MLC_Engine, SC_Engine, SC_EngineReception**: Implements specific signal combining algorithms and UART transmission logic.
  
- **Error Handling**:
  - Includes an error handler (`Error_Handler`) for critical errors.

## License

This software is licensed under terms that can be found in the LICENSE file in the root directory of this software component.

<div align="center">
  <a href="https://maazsalman.org/">
    <img width="70" src="click-svgrepo-com.svg" alt="gh" />
  </a>
  <p> Explore More! 🚀</p>
</div>

