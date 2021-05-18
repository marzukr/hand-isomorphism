add_library(
    handisomorphism SHARED
    check-main.c
    deck.c
    deck.h
    hand_index-impl.h
    hand_index.c
    hand_index.h
    )

set_property(TARGET handisomorphism PROPERTY C_STANDARD 99)
get_target_property(target_options handisomorphism COMPILE_OPTIONS)
list(REMOVE_ITEM target_options "-Werror")
set_property(TARGET handisomorphism PROPERTY COMPILE_OPTIONS ${target_options})
