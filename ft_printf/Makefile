# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: pgrellie <marvin@42.fr>                    +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2023/11/28 17:57:49 by pgrellie          #+#    #+#              #
#    Updated: 2023/12/07 15:01:42 by pgrellie         ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

NAME	= libftprintf.a

CC	= gcc
RM	= rm -f
AR	= ar rc
RN 	= ranlib

CFLAGS	= -Wall -Wextra -Werror

SRCS	= ft_utils.c\
		ft_printf.c\
		ft_putptr.c\
		ft_putunbr.c\

OBJS	= $(SRCS:.c=.o)

all: $(NAME)

$(NAME):
	$(CC) $(CFLAGS) -c $(SRCS)
	$(AR) $(NAME) $(OBJS)
	$(RN) $(NAME)

clean:
	$(RM) $(OBJS)

fclean: clean
	$(RM) $(NAME)

re: fclean all

.PHONY: all clean flean re
