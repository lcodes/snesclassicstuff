cmake_minimum_required(VERSION 2.6)
project(serverstuff)
project(testclient)
set(C_STANDARD_REQUIRED 99)
set(CMAKE_C_FLAGS  "${CMAKE_C_FLAGS} -Werror")
add_executable(serverstuff server.c cmd.c)
add_executable(testclient client.c)

install(TARGETS serverstuff RUNTIME DESTINATION bin)
