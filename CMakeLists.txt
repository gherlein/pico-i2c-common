add_library( pico_i2c_common
    pico_i2c_common.c
    pico_i2c_common.h
    )

target_link_libraries(pico_i2c_common
    pico_stdlib
    pico_multicore
    hardware_irq
    hardware_i2c
)

target_include_directories(pico_i2c_common 
    PUBLIC "${CMAKE_CURRENT_SOURCE_DIR}"
)

