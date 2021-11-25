cmake_minimum_required(VERSION 3.13)
set(CMAKE_CXX_STANDARD 11)

# Put your project name here
project(template)

# Add the directories where the dependencies can be found
add_subdirectory(Google_tests)
add_subdirectory(dependencies/glew-2.1.0/build/cmake)

#Directories to look for source code
include_directories(dependencies/glfw-3.3.5/include)
include_directories(dependencies/glew-2.1.0/include)
include_directories(dependencies/glm)

#Creates the executable target
add_executable(template main.cpp)

# Link the dependencies with the project.
target_link_libraries(template glfw ${OPENGL_glu_LIBRARY} ${GLFW_LIBRARIES} glew)
