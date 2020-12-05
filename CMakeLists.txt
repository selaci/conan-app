CMAKE_MINIMUM_REQUIRED(VERSION 3.17.2)
PROJECT(App)

add_definitions("-std=c++11")

include(${CMAKE_BINARY_DIR}/conanbuildinfo.cmake)
conan_basic_setup()

ADD_EXECUTABLE(app main.cpp)
target_link_libraries(app ${CONAN_LIBS})
