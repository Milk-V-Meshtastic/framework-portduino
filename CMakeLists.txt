cmake_minimum_required(VERSION 3.17)
project(Portduino)

set(CMAKE_CXX_STANDARD 14)

include_directories(cores/arduino/api)
include_directories(cores/portduino)
include_directories(cores/portduino/FS)

add_executable(Portduino
        cores/arduino/api/deprecated/Client.h
        cores/arduino/api/deprecated/HardwareSerial.h
        cores/arduino/api/deprecated/IPAddress.h
        cores/arduino/api/deprecated/Print.h
        cores/arduino/api/deprecated/Printable.h
        cores/arduino/api/deprecated/Server.h
        cores/arduino/api/deprecated/Stream.h
        cores/arduino/api/deprecated/Udp.h
        cores/arduino/api/deprecated/WString.h
        cores/arduino/api/deprecated-avr-comp/avr/dtostrf.h
        cores/arduino/api/deprecated-avr-comp/avr/interrupt.h
        cores/arduino/api/deprecated-avr-comp/avr/pgmspace.h
        cores/arduino/api/ArduinoAPI.h
        cores/arduino/api/Binary.h
        cores/arduino/api/Client.h
        cores/arduino/api/Common.cpp
        cores/arduino/api/Common.h
        cores/arduino/api/Compat.h
        cores/arduino/api/HardwareI2C.h
        cores/arduino/api/HardwareSerial.h
        cores/arduino/api/HardwareSPI.h
        cores/arduino/api/Interrupts.h
        cores/arduino/api/IPAddress.cpp
        cores/arduino/api/IPAddress.h
        cores/arduino/api/itoa.h
        # cores/arduino/api/PluggableUSB.cpp
        # cores/arduino/api/PluggableUSB.h
        cores/arduino/api/Print.cpp
        cores/arduino/api/Print.h
        cores/arduino/api/Printable.h
        cores/arduino/api/RingBuffer.h
        cores/arduino/api/Server.h
        cores/arduino/api/Stream.cpp
        cores/arduino/api/Stream.h
        cores/arduino/api/String.cpp
        cores/arduino/api/String.h
        cores/arduino/api/Udp.h
        cores/arduino/api/USBAPI.h
        cores/arduino/api/WCharacter.h
        cores/portduino/Arduino.h
        cores/portduino/itoa.cpp
        cores/portduino/dtostrf.c
        cores/portduino/main.cpp
        cores/portduino/linux/millis.cpp
        cores/portduino/simulated/SimCommon.cpp
        cores/portduino/Utility.cpp
        cores/portduino/Utility.h
        cores/portduino/simulated/SimHardwareSPI.cpp
        example/test.cpp
       	cores/portduino/simulated/SimHardwareI2C.cpp
       	cores/portduino/simulated/SimHardwareI2C.h
       	cores/portduino/linux/LinuxCommon.cpp
       	cores/portduino/linux/LinuxSerial.cpp
        cores/portduino/linux/LinuxSerial.h
        cores/portduino/linux/LinuxHardwareI2C.cpp
       	cores/portduino/linux/LinuxHardwareI2C.h)
