# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: egermen <egermen@student.42kocaeli.com.    +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2024/01/05 14:45:53 by egermen           #+#    #+#              #
#    Updated: 2024/01/05 14:45:54 by egermen          ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

NAME            =   minitalk

SERVER			=	server
SERVER_SRC		=	server.c


CLIENT			=	client
CLIENT_SRC		=	client.c


UTILS_SRC		=	utils.c 

CC				=	gcc
RM 				=	rm -rf
FLAGS			= 	-Wall -Werror -Wextra

all : $(SERVER) $(CLIENT)

$(NAME): all

$(SERVER) :
	$(CC) $(FLAGS) $(SERVER_SRC) $(UTILS_SRC) -o $(SERVER)


$(CLIENT) :
	$(CC) $(FLAGS) $(CLIENT_SRC) $(UTILS_SRC) -o $(CLIENT)

clean :
	$(RM) $(SERVER) $(CLIENT)

fclean :
	$(RM) $(SERVER) $(CLIENT)

re : fclean all

.PHONY: all clean fclean re 