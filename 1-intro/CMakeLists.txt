project(1-version)
add_executable(${PROJECT_NAME} version.cpp)
target_link_libraries(${PROJECT_NAME} Qt5::Core)

#add_executable(helloworld
#    mainwindow.ui
#    mainwindow.cpp
#    main.cpp
#    resources.qrc
#)
#
#target_link_libraries(helloworld Qt5::Widgets)
