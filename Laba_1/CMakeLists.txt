cmake_minimum_required(VERSION 2.8) 

project(Laba_1)

include_directories(include)

set(SOURCE tests/main.cpp)

set(SOURCE_LIB sources/Source.cpp)

add_library(test STATIC ${SOURCE_LIB})

add_executable(main ${SOURCE})

target_link_libraries(main test)		
					