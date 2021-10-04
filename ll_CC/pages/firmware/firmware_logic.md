# Firmware Design Logic

## Introduction

In this firmware design. The main program will only used to initialize internal registers. Main things for MCU to do are all in interrupt handle codes.

## main.c

In "main" function, serveral functions are called to initialize the MCU's devices including ADC, DAC, USB modules and External devices such as AFE, PSU.

## Interrupt

To be edited