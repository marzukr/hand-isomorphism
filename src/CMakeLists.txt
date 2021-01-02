cmake_minimum_required(VERSION 3.5.0)
project(handisomorphism)

add_library(
    ${PROJECT_NAME} SHARED
    check-main.c
    deck.c
    deck.h
    hand_index-impl.h
    hand_index.c
    hand_index.h
    )

set_property(TARGET ${PROJECT_NAME} PROPERTY C_STANDARD 99)