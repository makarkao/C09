SRCS		= srcs/ft_putchar.c srcs/ft_swap.c srcs/ft_putstr.c srcs/ft_strlen.c srcs/ft_strcmp.c
OBJECTS	= ft_putchar.o ft_swap.o ft_putstr.o ft_strlen.o ft_strcmp.o

FLAGS=-Wall -Wextra -Werror
GCC =gcc
INCLUDES =./includes
LIBC =ar rc
BIN=libft.a
PRE=./srcs/

all : $(BIN)

$(BIN) : $(OBJECTS)
	$(LIBC) $(BIN) $(OBJECTS)
	ranlib $(BIN)

$(OBJECTS): $(SRCS) $(INCLUDES)
	$(GCC) $(FLAGS) -I$(INCLUDES) -c $(SRCS)
	


clean :
	rm -rf $(OBJECTS)

fclean : clean
	rm -rf $(BIN)

re : fclean all
