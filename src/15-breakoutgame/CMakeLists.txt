add_exe(main.cpp paddle.cpp paddle.h brick.cpp brick.h ball.cpp ball.h breakout.cpp breakout.h)

file(COPY brickie.png ball.png paddle.png DESTINATION ${CMAKE_CURRENT_BINARY_DIR})
