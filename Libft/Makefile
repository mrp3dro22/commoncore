# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: pfranco- <pfranco-@student.42.fr>          +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2023/10/16 15:18:24 by pfranco-          #+#    #+#              #
#    Updated: 2023/11/24 12:50:10 by pfranco-         ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

NAME = libft.a
FLAGS = -Wall -Wextra -Werror
SRC =	ft_isalpha.c ft_isdigit.c ft_isalnum.c ft_isascii.c ft_isprint.c ft_strlen.c \
		ft_memset.c ft_bzero.c ft_memcpy.c ft_memmove.c ft_strlcpy.c \
		ft_strlcat.c ft_toupper.c ft_tolower.c ft_strchr.c ft_strrchr.c ft_strncmp.c \
		ft_memchr.c ft_strnstr.c ft_atoi.c ft_calloc.c ft_strdup.c ft_substr.c \
		ft_strjoin.c ft_strtrim.c ft_split.c ft_itoa.c ft_strmapi.c ft_putchar_fd.c \
		ft_putstr_fd.c ft_putendl_fd.c ft_putnbr_fd.c ft_striteri.c  ft_memcmp.c

BONUS =		ft_lstadd_back.c ft_lstadd_front.c ft_lstclear.c ft_lstdelone.c ft_lstlast.c ft_lstnew.c ft_lstsize.c \
			ft_lstiter.c ft_lstmap.c

OBJECTS_SRC = $(SRC:.c=.o)
OBJECTS_BONUS = $(BONUS:.c=.o)

.PHONY: all clean fclean re bonus

all: $(NAME)

$(NAME): 
	cc -c $(FLAGS) $(SRC)
	ar rs $(NAME) $(OBJECTS_SRC)

bonus:
	cc -c $(FLAGS) $(BONUS)
	ar rs $(NAME) $(OBJECTS_BONUS)

clean:
	rm -f $(OBJECTS_SRC) $(OBJECTS_BONUS)

fclean: clean
	rm -f $(NAME)

re: fclean all