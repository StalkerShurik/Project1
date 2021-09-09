cmake_minimum_required(VERSION 3.0)

project(Project1)

set(CMAKE_CXX_STANDARD 20)

set(OPTIM "-O3 -march=native")
#set(DEFFLG "-pthread")
set(DEBFLG "${DEFFLG} -Wall -Wextra -Werror -Wunused -Wunused-value")
#set(SANIT "-fsanitize=address -static-libasan -fsanitize=leak -fsanitize=undefined -fno-omit-frame-pointer")

#set(ALLDEF "${OPTIM} ${DEFFLG}")
#set(ALLDEB "${ALLDEF} ${DEBFLG}")

#set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} ${ALLDEB} ${SANIT}")

add_executable(Project1 main.cpp)