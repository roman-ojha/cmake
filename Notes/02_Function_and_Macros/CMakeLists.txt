# first we will include the cmake version
# try to use that version or less then the version that you currently have in you computer
cmake_minimum_required(VERSION 3.26.0)

# now we will add the project name
project(TEST)
# we can also provide the langauge that we use
# project(TEST LANGUAGE CXX)

# now we will provide the executable name that we want build
# also have to provide the source file name
add_executable(${PROJECT_NAME} main.cpp)
# add_executable(<build_name> <source_name>)