# Project properties
cmake_minimum_required(VERSION 3.28.1)
project(PROJECT-NAME)
set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

# Find packages
# find_package(package CONFIG REQUIRED)

# Create executable
file(GLOB SRC_FILES "src/*.cpp")
add_executable(${PROJECT_NAME} ${SRC_FILES})

# Include directories
target_include_directories(
    ${PROJECT_NAME}
    PRIVATE
)

# Link libraries
target_link_libraries(
    ${PROJECT_NAME}
    PRIVATE
)