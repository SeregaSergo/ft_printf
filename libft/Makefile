# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: bswag <marvin@42.fr>                       +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2020/11/09 14:09:47 by bswag             #+#    #+#              #
#    Updated: 2020/12/23 20:40:04 by bswag            ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

NAME = libft.a
SRCS = ft_strlcat.c \
	   ft_isprint.c \
	   ft_toupper.c \
	   ft_tolower.c \
	   ft_strlcpy.c \
	   ft_isascii.c \
	   ft_isdigit.c \
	   ft_isalnum.c \
	   ft_isalpha.c \
	   ft_strlen.c \
	   ft_bzero.c \
	   ft_strchr.c \
	   ft_strrchr.c \
	   ft_strncmp.c \
	   ft_strnstr.c \
	   ft_atoi.c \
	   ft_memset.c \
	   ft_memcpy.c \
	   ft_memccpy.c \
	   ft_memmove.c \
	   ft_memchr.c \
	   ft_memcmp.c \
	   ft_calloc.c \
	   ft_strdup.c \
	   ft_substr.c \
	   ft_strjoin.c \
	   ft_strtrim.c \
	   ft_split.c \
	   ft_itoa.c \
	   ft_strmapi.c \
	   ft_putchar_fd.c \
	   ft_putstr_fd.c \
	   ft_putendl_fd.c \
	   ft_putnbr_fd.c \
	   ft_itoa_base.c \
	   ft_strtoupper.c \
	   ft_lutoa_base.c \
	   ft_write_param.c \
	   ft_strchr_null.c
SRCSBNS = ft_lstnew.c \
		  ft_lstadd_front.c \
		  ft_lstsize.c \
		  ft_lstlast.c \
		  ft_lstadd_back.c \
		  ft_lstdelone.c \
		  ft_lstclear.c \
		  ft_lstiter.c \
		  ft_lstmap.c
OBJS = $(SRCS:%.c=%.o)
OBJSBNS = $(SRCSBNS:%.c=%.o)
CC = gcc
CFLAGS = -c -Wall -Wextra -Werror
DEPS = libft.h

.PHONY: all clean fclean re bonus

all: $(NAME)

$(NAME): $(OBJS)
	ar -rcs $(NAME) $(OBJS)

%.o: %.c $(DEPS)
	$(CC) $(CFLAGS) -c -o $@ $<

bonus: $(NAME) $(OBJSBNS)
	ar -rs $(NAME) $(OBJSBNS)

clean:
	/bin/rm -f $(OBJS) $(OBJSBNS)

fclean: clean
	/bin/rm -f $(NAME)

re: fclean all
