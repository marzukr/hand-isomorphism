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
get_target_property(target_options ${PROJECT_NAME} COMPILE_OPTIONS)
list(REMOVE_ITEM target_options "-Werror")
set_property(TARGET ${PROJECT_NAME} PROPERTY COMPILE_OPTIONS ${target_options})
