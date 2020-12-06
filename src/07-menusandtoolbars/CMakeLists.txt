
add_exe(01-main-simplemenu.cpp simplemenu.cpp simplemenu.h)
add_exe(02-main-anothermenu.cpp anothermenu.cpp anothermenu.h)
add_exe(03-main-checkablemenu.cpp checkable.cpp checkable.h)
add_exe(04-main-toolbar.cpp toolbar.cpp toolbar.h new.png open.png quit.png)
add_exe(05-main-skeleton.cpp skeleton.cpp skeleton.h new.png open.png quit.png)

file(COPY new.png DESTINATION ${CMAKE_CURRENT_BINARY_DIR})
file(COPY open.png DESTINATION ${CMAKE_CURRENT_BINARY_DIR})
file(COPY quit.png DESTINATION ${CMAKE_CURRENT_BINARY_DIR})
