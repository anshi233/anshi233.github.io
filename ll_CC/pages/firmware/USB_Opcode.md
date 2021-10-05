# USB User defined Opcode

## Introduction

In this project, A user defined opcode (16bits length) is used to send and receive instruction to/from USB host.
Following is the list of Opcode defined in the code.

## USB RX Opcode

|Opcode|Usage|
|------|-----|
|0x00|Reversed|
|0x01|Return status(looks like "Ping" the device) to Host|
|0x10|Set PSU|
|0x11|Disable PSU|
|0x24|receive ADC measure config|
|0x27|oscilloscope triger config|
|0x30|DAC waveform output config|
|0x31|DAC waveform output disable|
|0x40|Read ADC (not currently used)|
|0x42|Triggered ADC Reading (not currently used)|
|0x44|Read ADC Periodic (not currently used)|
|0x46|Dump ADC Data|
|0x48|Random Testing for ADC (not currently used)|
|0x50|Enable_ADC_Logging|
|0x51|Disable_ADC_Logging|


## USB RX Opcode (For Test)

TBD


## USB TX Opcode

These opcodes are hidded in every places...
They are discoverd by tracking call of "CDC_Transmit_HS" function in "usbd_cdc_if.c"


|Opcode|Usage|
|------|-----|
|0x43|ADC enough samples, Data sending?|
|0x47|Dump ADC Data Sending|
|0x52|ADC trigger Data sending?|

