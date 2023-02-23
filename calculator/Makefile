CC = gcc
CFLAGS = -Wall -Werror

SRC = main.c addition.c subtraction.c multiplication.c division.c
OBJ = $(SRC:.c=.o)

calculator: $(OBJ)
	$(CC) $(CFLAGS) -o calculator $(OBJ)

%.o: %.c operations.h
	$(CC) $(CFLAGS) -c $< -o $@

clean:
	rm -f $(OBJ) calculator

