# Generated Cmake Pico project file

cmake_minimum_required(VERSION 3.13)

set(CMAKE_C_STANDARD 11)
set(CMAKE_CXX_STANDARD 17)

# initalize pico_sdk from installed location
# (note this can come from environment, CMake cache etc)
# set(PICO_SDK_PATH "/YOUR_PICO_SDK_PATH/pico-sdk")

# Pull in Pico SDK (must be before project)
include(pico_sdk_import.cmake)

project(pico-pwm-audio C CXX ASM)

set(PICO_CXX_ENABLE_EXCEPTIONS 1)

set(PICO_CXX_ENABLE_RTTI 1)

# Initialise the Pico SDK
pico_sdk_init()

# Add executable. Default name is the project name, version 0.1

add_executable(pico-pwm-audio pico-pwm-audio.c )

pico_set_program_name(pico-pwm-audio "pico-pwm-audio")
pico_set_program_version(pico-pwm-audio "0.1")

pico_enable_stdio_uart(pico-pwm-audio 1)
pico_enable_stdio_usb(pico-pwm-audio 0)

# Add the standard library to the build
target_link_libraries(pico-pwm-audio pico_stdlib)

# Add any user requested libraries
target_link_libraries(pico-pwm-audio
        hardware_dma
        hardware_pio
        hardware_timer
        hardware_clocks
        hardware_pwm
        )

pico_add_extra_outputs(pico-pwm-audio)

