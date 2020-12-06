cmake_minimum_required(VERSION 3.14)

project(helloworld)

macro(add_exe name)
	# name of exe is equal to  prefix + name of first source file without extension
	# get prefix, that is, the name of current directory
	get_filename_component(prefix ${CMAKE_CURRENT_LIST_DIR} NAME)
	string(REPLACE " " "_" prefix ${prefix})
	# remove extension of first source file
	get_filename_component(name_noext ${name} NAME_WE)
	# put together name of executable, name is equal to the first, and sometimes the only, element in ${ARGV}
	add_executable(${prefix}-${name_noext} ${ARGV})
	target_link_libraries(${prefix}-${name_noext} Qt5::Core Qt5::Gui Qt5::Widgets)
endmacro()

set(CMAKE_AUTOMOC ON)
set(CMAKE_AUTORCC ON)
set(CMAKE_AUTOUIC ON)

if(CMAKE_VERSION VERSION_LESS "3.7.0")
    set(CMAKE_INCLUDE_CURRENT_DIR ON)
endif()

find_package(Qt5 COMPONENTS Core Widgets REQUIRED)

add_subdirectory(src/01-intro)
add_subdirectory(src/02-strings)
add_subdirectory(src/03-date-time)
add_subdirectory(src/04-containers)
add_subdirectory(src/05-files)
add_subdirectory(src/06-firstprograms)
add_subdirectory(src/07-menusandtoolbars)
add_subdirectory(src/08-layout)
add_subdirectory(src/09-eventsandsignals)
add_subdirectory(src/10-widgets)
add_subdirectory(src/11-widgets2)
add_subdirectory(src/12-painting)
add_subdirectory(src/13-customwidget)
add_subdirectory(src/14-snake)
add_subdirectory(src/15-breakoutgame)
