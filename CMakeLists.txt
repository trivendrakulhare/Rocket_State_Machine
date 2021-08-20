cmake_minimum_required(VERSION 3.0.0)
project(stateMachine VERSION 1.0)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED True)

add_executable(stateMachine ../src/main.cpp
                                src/CountDown.cpp
                                src/FairingJettison.cpp
                                src/LaunchPadRelease.cpp
                                src/NextEngine.cpp
                                src/InitialEngineIgnition.cpp
                                src/Termination.cpp
                                src/PayloadRealease.cpp) 
                                
target_include_directories(stateMachine PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}/include)