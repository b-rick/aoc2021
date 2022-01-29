file(GLOB HEADER_LIST CONFIGURE_DEPENDS "${PROJECT_SOURCE_DIR}/include/*.h")
file(GLOB SOURCE_FILES ./*)

add_library(Library SHARED ${SOURCE_FILES} ${HEADER_LIST})
target_include_directories(Library PUBLIC "../include")