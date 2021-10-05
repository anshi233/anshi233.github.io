# Interrupt definition

## Introduction
In this Project, most of the logic is done in interrupt.

## Interrupt device list
Following list shows the device that using interrupt in this project.

- ADC1 and ADC2

- DMA (no user code is used)

- Timer (see [Timer Definition](timer_definition.md))

## Interrupt Handler Functions And File Location

**ADC1 and ADC2**:


**Timer**:
All timer related interrupts are processed in "HAL_TIM_PeriodElapsedCallback0" in "main.c"
Notice that TIM17 is not used but somehow its codes are not deleted.
The detailed handle logic can see in wiki's device page.