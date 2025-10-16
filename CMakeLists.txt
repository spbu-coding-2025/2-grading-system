cmake_minimum_required(VERSION 3.17)
project(tests LANGUAGES C ASM)

set(CMAKE_C_STANDARD 99)
set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -Wall -Wextra -pedantic -Werror")

if (IS_DIRECTORY ${STUDENT_DIR})
    set(STUDENT_SOURCE_DIR "${STUDENT_DIR}/src")
    add_subdirectory(${STUDENT_SOURCE_DIR})
endif()
