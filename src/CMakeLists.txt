add_library(${CMAKE_PROJECT_NAME} main.cpp)

asteroid_app_qml_module(${CMAKE_PROJECT_NAME}
	main.qml
)

target_link_libraries(
	${CMAKE_PROJECT_NAME}
	PUBLIC
		Asteroid::AsteroidApp6
)

install(
	TARGETS ${CMAKE_PROJECT_NAME}
	DESTINATION ${CMAKE_INSTALL_LIBDIR}
)
