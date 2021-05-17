cmake_minimum_required(VERSION 3.6.0)

project(asteroid-helloworld
	VERSION 0.0.1
	DESCRIPTION "Sample application to get started on Asteroid")

find_package(ECM REQUIRED NO_MODULE)
find_package(AsteroidApp REQUIRED)

set(CMAKE_MODULE_PATH ${ECM_MODULE_PATH} ${ASTEROID_MODULE_PATH})

include(FeatureSummary)
include(GNUInstallDirs)
include(ECMQMLModules)
include(AsteroidCMakeSettings)
include(AsteroidTranslations)

add_subdirectory(src)

generate_desktop(${CMAKE_SOURCE_DIR} asteroid-helloworld)

feature_summary(WHAT ALL FATAL_ON_MISSING_REQUIRED_PACKAGES)
