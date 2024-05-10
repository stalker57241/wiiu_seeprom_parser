cmake_minimum_required(VERSION 3.10)

project(wiiu_seeprom_parser LANGUAGES C)

add_library(aes "src/aes.c")

add_executable(seeprom_parser "src/wiiu_seeprom_parser.c")
target_link_libraries(seeprom_parser aes)
