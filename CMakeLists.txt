add_library( pico-i2c-common
    pico-i2c-common.c
    pico-i2c-common.h
    )

target_link_libraries(pico-i2c-common
    pico_stdlib
    pico_multicore
    hardware_irq
    hardware_i2c
)

target_include_directories(pico-i2c-common 
    PUBLIC "${CMAKE_CURRENT_SOURCE_DIR}"
)

