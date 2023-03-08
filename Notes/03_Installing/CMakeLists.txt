cmake_minimum_required(VERSION 3.26.0)

project(Test)

add_executable(${PROJECT_NAME} main.cpp)


# installing executable to sepcific directory command:
# in target we have to sepcify the executable name
# and it will install in destination '${PROJECT_BINARY_DIR}/bin' means in './build/bin'
install(TARGETS Test  DESTINATION ${PROJECT_BINARY_DIR}/bin) # didnot work in windows right now
# to run the install we have to first build cmake:
# -> cmake -S . -B build -G "Unix Makefiles"
# -> cd build
# -> make install