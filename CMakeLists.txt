set(RELIABLE_SOURCES 
    reliable.c
)

file(GLOB RELIABLE_INCLUDE_FILES "reliable.h")

add_library(reliable STATIC ${RELIABLE_SOURCES})

target_link_libraries(reliable)

install_our_headers(${RELIABLE_INCLUDE_FILES})

set(RELIABLE_LINK_WITH reliable PARENT_SCOPE)

#-----------------------------------------------------------------------------#
# vim: set ts=8 sts=4 sw=4 et:
