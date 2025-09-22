# Copyright (c) 2024 ARM Limited. All rights reserved.
# SPDX-License-Identifier: Apache-2.0

add_library(mbed-stm32l4a6vg INTERFACE)

target_sources(mbed-stm32l4a6vg
    INTERFACE
    PeripheralPins.c
)

target_include_directories(mbed-stm32l4a6vg
    INTERFACE
    .
)

target_link_libraries(mbed-stm32l4a6vg INTERFACE mbed-stm32l4a6xg)
