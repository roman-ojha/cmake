cmake_minimum_required(VERSION 3.26.0)

project(TEST)

add_executable(${PROJECT_NAME} main.cpp)

# message function to print console
message("Hello world")
# printing varialbe values
message("${PROJECT_NAME}")

# Now we will create our own 'print()'
# creating own function
# function(<name_of_function_that_we_want_to_callable_with> <arguments>)
function(print var)
    # var is the referencing varialbe
    # in this example we get 'PROJECT_NAME'
    # we can dreference the referencing varialbe to get the variable value like of 'PROJECT_NAME'
    # ${${var}}
    message("${var} = ${${var}}") # PROJECT_NAME = TEST
endfunction()

print(PROJECT_NAME)

# now we can print any varialbes
print(CMAKE_PROJECT_NAME)
# Start from here: https://youtu.be/4BvyJGfFKNg?list=PL8i3OhJb4FNV10aIZ8oF0AA46HgA2ed8g&t=388
