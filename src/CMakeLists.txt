add_library(asteroid-helloworld main.cpp resources.qrc)

target_link_libraries(asteroid-helloworld PUBLIC
	AsteroidApp)

install(TARGETS asteroid-helloworld
	DESTINATION ${CMAKE_INSTALL_LIBDIR})
