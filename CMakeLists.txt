cmake_minimum_required(VERSION 3.12)

include(pico_sdk_import.cmake)
project(your_project_name C CXX ASM)

pico_sdk_init()

# Add your source files here
add_executable(your_project_name
    your_project_name.c
)

target_link_libraries(your_project_name
    pico_stdlib
)

# Enable USB output, disable UART output by default
pico_enable_stdio_usb(your_project_name 1)
pico_enable_stdio_uart(your_project_name 0)

# Enable extra outputs (optional)
pico_add_extra_outputs(your_project_name)
