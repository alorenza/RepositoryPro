# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: alorenza <alorenza@student.42malaga.com    +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2023/09/16 15:37:46 by alorenza          #+#    #+#              #
#    Updated: 2023/10/19 12:34:35 by alorenza         ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

NAME = libft.a 

SRCS = ft_atoi.c ft_bzero.c ft_isalnum.c ft_isalpha.c\
		ft_isascii.c ft_isdigit.c ft_isprint.c ft_memchr.c\
		ft_memcmp.c ft_memcpy.c ft_memmove.c ft_memset.c\
		ft_strchr.c ft_strlcpy.c ft_strlen.c\
		ft_strncmp.c ft_strrchr.c ft_tolower.c ft_toupper.c\
		ft_strlcat.c ft_strchr.c ft_strnstr.c ft_calloc.c\
		ft_strdup.c ft_substr.c ft_strjoin.c ft_strtrim.c\
		ft_itoa.c ft_strmapi.c ft_striteri.c ft_putchar_fd.c\
		ft_putstr_fd.c ft_putendl_fd.c ft_putnbr_fd.c ft_lstnew.c\
		ft_lstadd_front.c ft_lstsize.c ft_lstlast.c ft_lstadd_back.c\
		ft_lstdelone.c ft_lstclear.c ft_lstiter.c ft_lstmap.c\
		ft_split.c


OBJ = $(SRCS:.c=.o)
OBJ_BONUS = $(SOURCE_BONUS:.c=.o)
CC = gcc
CFLAGS = -Wall -Wextra -Werror
LIB = ar rcs
all: $(NAME)
$(NAME): $(OBJ)
	$(LIB) $(NAME) $(OBJ)
$(OBJ): $(SRCS)
	$(CC) $(CFLAGS) -c $(SRCS)
clean:
	rm -f $(OBJ) $(OBJ_BONUS)
fclean: clean
	rm -rf $(NAME)
re: fclean all
bonus: $(OBJ) $(OBJ_BONUS)
	$(LIB) $(NAME) $(OBJ) $(OBJ_BONUS)
.PHONY: re all clean fclean bonus