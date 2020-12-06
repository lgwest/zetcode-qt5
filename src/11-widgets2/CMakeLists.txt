file(COPY bojnice.jpg DESTINATION ${CMAKE_CURRENT_BINARY_DIR})

add_exe(1-main-checkbox.cpp checkbox.cpp checkbox.h)
add_exe(2-main-listwidget.cpp listwidget.cpp listwidget.h)
add_exe(3-main-progressbar.cpp progressbar.cpp progressbar.h)
add_exe(4-main-pixmap.cpp pixmap.cpp pixmap.h)
add_exe(5-main-splitter.cpp splitter.cpp splitter.h)
add_exe(6-main-table.cpp table.cpp table.h)
