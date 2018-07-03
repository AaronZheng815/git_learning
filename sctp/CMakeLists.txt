cmake_minimum_required(VERSION 2.8)

project(mysctp)

add_definitions("-g -Wall")

add_executable(sctp_clt sctp_clt.c)
target_link_libraries(sctp_clt sctp)

add_executable(sctp_ser sctp_ser.c)
target_link_libraries(sctp_ser sctp)

add_executable(sctp_echo sctp_ser_1.c)
target_link_libraries(sctp_echo sctp)

add_executable(echo_c sctp_clt_1.c)
target_link_libraries(echo_c sctp)