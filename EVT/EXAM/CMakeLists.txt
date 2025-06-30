cmake_minimum_required(VERSION 3.22)
add_library(ch32v30x)
target_sources(ch32v30x
    SRC/Core/core_riscv.c
    SRC/Peripheral/src/ch32v30x_adc.c
    SRC/Peripheral/src/ch32v30x_bkp.c
    SRC/Peripheral/src/ch32v30x_can.c
    SRC/Peripheral/src/ch32v30x_crc.c
    SRC/Peripheral/src/ch32v30x_dac.c
    SRC/Peripheral/src/ch32v30x_dbgmcu.c
    SRC/Peripheral/src/ch32v30x_dma.c
    SRC/Peripheral/src/ch32v30x_dvp.c
    SRC/Peripheral/src/ch32v30x_eth.c
    SRC/Peripheral/src/ch32v30x_exti.c
    SRC/Peripheral/src/ch32v30x_flash.c
    SRC/Peripheral/src/ch32v30x_fsmc.c
    SRC/Peripheral/src/ch32v30x_gpio.c
    SRC/Peripheral/src/ch32v30x_i2c.c
    SRC/Peripheral/src/ch32v30x_iwdg.c
    SRC/Peripheral/src/ch32v30x_misc.c
    SRC/Peripheral/src/ch32v30x_opa.c
    SRC/Peripheral/src/ch32v30x_pwr.c
    SRC/Peripheral/src/ch32v30x_rcc.c
    SRC/Peripheral/src/ch32v30x_rng.c
    SRC/Peripheral/src/ch32v30x_rtc.c
    SRC/Peripheral/src/ch32v30x_sdio.c
    SRC/Peripheral/src/ch32v30x_spi.c
    SRC/Peripheral/src/ch32v30x_tim.c
    SRC/Peripheral/src/ch32v30x_usart.c
    SRC/Peripheral/src/ch32v30x_wwdg.c
    SRC/Startup/startup_ch32v30x_D8.S
)

target_link_libraries(ch32v30x PUBLIC
    SRC/Core
    SRC/Peripheral/inc
)
