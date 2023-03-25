cmake_minimum_required(VERSION 3.10.2 FATAL_ERROR)


project(cmake
    VERSION 0.0.1
    DESCRIPTION  "ubuntu cmake demo"
    HOMEPAGE_URL  "https://github.com/wulichengxu"
    LANGUAGES      C CXX

)

list(APPEND CMAKE_MODULE_PATH"${CMAKE_SOURCE_DIR}/cmake")
include(Build_Info)

add_subdirectory(external)
add_subdirectory(src)
add_subdirectory(docs)
add_subdirectory(test)
add_subdirectory(packaging)


