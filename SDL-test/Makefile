## Simple SDL mini code
 
CC=gcc
 
CPPFLAGS= `pkg-config --cflags sdl` -MMD
CFLAGS= -Wall -Wextra -Werror -std=c99 -O3
LDFLAGS=
LDLIBS= `pkg-config --libs sdl` -lSDL_image
 
OBJ= pixel_operations.o image_process.o to_matrice.o main.o
DEP= ${OBJ:.o=.d}
 
all: main
 
main: ${OBJ}
 
clean:
	${RM} ${OBJ} ${DEP} *~
	${RM} main
 
-include ${DEP}
 
# END
