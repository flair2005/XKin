project( posture )
file( GLOB SOURCES "*.c" )

add_library( ${PROJECT_NAME} SHARED ${SOURCES} "const.h" ) 
target_link_libraries( ${PROJECT_NAME} ${OpenCV_LIBS} ${FFTW_LIBRARIES} )

