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
set_target_properties(handisomorphism PROPERTIES COMPILE_FLAGS "-w")
