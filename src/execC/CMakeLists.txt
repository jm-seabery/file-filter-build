# Set the project name (this is the final exec name)
project (test-C)

set ( SOURCES_CPP
	${PROJECT_SOURCE_DIR}/classC.h
	${PROJECT_SOURCE_DIR}/main.cpp
)

# Create folders in the IDE
source_group(TREE ${CMAKE_CURRENT_SOURCE_DIR} FILES ${SOURCES_CPP} )

# Add this exec
add_executable(${PROJECT_NAME} ${SOURCES_CPP} )

include_directories(${PROJECT_SOURCE_DIR})
