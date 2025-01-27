# Timer Definition

## Introduction
Many timers are used in this project. In this page, information of timers are listed.
STM32CubeMX is used to arrange information of timer.
In "main.c", "HAL_TIM_PeriodElapsedCallback" is used to handle all interrupt generated by timers.

## List of Enabled Timers By Name

   |Timer|Interrupt|Prescaler|Counter Period|frequency(Hz)|usage|
   |-----|---------|---------|--------------|-------------|-----|
   |TIM1|No|48-1|100-1|TBD|DAC1_Out1|
   |TIM2|No|48-1|100-1|TBD|DAC1_Out2|
   |TIM3|No|48-1|2-1|TBD|ADC1|
   |TIM4|Yes|480-1|2-1|TBD|ADC1 Enough Samples after the triggered encountered|
   |TIM5|Yes|960-1|2-1 (variable)|variable|ADC1 Periodic Timer Trigger|
   |TIM6|Yes|480-1|100-1|TBD|ADC2 Enough Samples after the triggered encountered|
   |TIM7|Yes|960-1|2-1 (variable)|variable|ADC2 Periodic Timer Trigger|
   |TIM8|Yes (update with TIM13)|48-1|2-1|TBD|ADC2|
   |TIM13|Yes|200-1|20-1|TBD|USB Tx (ADC)|
   |TIM15|Yes|550-1|100-1|TBD|TBD|
   |TIM16|Yes|200-1|20-1|TBD|USB Polling timer|
   |TIM17|No|Not avaliable|Not avaliable|1000Hz| uwTick vatiable(not used)|
   |TIM24|Yes|480-1|500-1|TBD|TBD|