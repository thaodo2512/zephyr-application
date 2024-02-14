# Minimum required version of CMake
cmake_minimum_required(VERSION 3.20)

# Set the project name
project(zephyr-application)

# Set the Zephyr base directory
set(ZEPHYR_BASE $ENV{ZEPHYR_BASE})

# Include the Zephyr CMake module
include(${ZEPHYR_BASE}/cmake/app/boilerplate.cmake NO_POLICY_SCOPE)

# Add your source files here
target_sources(app PRIVATE
    src/main.c
)
