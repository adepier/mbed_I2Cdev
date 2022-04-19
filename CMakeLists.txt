 
set(I2C_SOURCES I2Cdev.cpp) 
add_library(mbed_I2Cdev STATIC ${PID_SOURCES})
target_link_libraries( mbed_I2Cdev mbed-os)

set(I2C_HEADER_DIR ${CMAKE_CURRENT_SOURCE_DIR} )
target_include_directories(mbed_I2Cdev PUBLIC ${I2C_HEADER_DIR})