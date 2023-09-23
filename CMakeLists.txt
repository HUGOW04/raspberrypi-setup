 cmake_minimum_required(VERSION 3.14)
set(PICO_BOARD pico_w)
include(pico_sdk_import.cmake)

project(pico)

pico_sdk_init()

add_executable(pico
    main.c
)


# Add pico_stdlib library, add more if used
target_link_libraries(pico pico_stdlib pico_cyw43_arch_none)

pico_add_extra_outputs(pico)
