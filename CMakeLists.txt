cmake_minimum_required(VERSION 3.10)

project(Piano)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -O2")
set(CMAKE_EXE_LINKER_FLAGS "${CMAKE_EXE_LINKER_FLAGS} -mwindows")

include(FetchContent)
FetchContent_Declare(
	sfml
	GIT_REPOSITORY "http://github.com/SFML/SFML"
	GIT_TAG 2.6.1
)

FetchContent_MakeAvailable(sfml)

include_directories(${PROJECT_SOURCE_DIR}/include)

file(GLOB SRC_FILES "src/*.cpp")
add_executable(${PROJECT_NAME} ${SRC_FILES})

target_link_libraries(${PROJECT_NAME} PRIVATE sfml-graphics sfml-window sfml-system sfml-audio)
