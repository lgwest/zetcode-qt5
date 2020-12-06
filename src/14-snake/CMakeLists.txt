file(COPY dot.png head.png apple.png DESTINATION ${CMAKE_CURRENT_BINARY_DIR})

add_exe(main.cpp snake.cpp snake.h dot.png head.png apple.png)
