cmake_minimum_required(VERSION 3.26.0)

project(Test)

add_executable(${PROJECT_NAME} main.cpp)

install(TARGETS Test  DESTINATION ${PROJECT_BINARY_DIR}/bin)
# Currently on :https://youtu.be/DDHCEE_PHOU?list=PLalVdRk2RC6o5GHu618ARWh0VO0bFlif4&t=728