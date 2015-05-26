if (PLATFORM STREQUAL "iotlab-a8-m3")
add_executable(iw1_a8_m3 main)
target_link_libraries(iw1_a8_m3 platform mac_csma)

else (PLATFORM STREQUAL "iotlab-a8-m3")
add_executable(iw1_m3 main)
target_link_libraries(iw1_m3 platform lps331ap isl29020 mac_csma)
endif (PLATFORM STREQUAL "iotlab-a8-m3")
