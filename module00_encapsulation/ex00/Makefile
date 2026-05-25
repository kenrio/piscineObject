# **************************************************************************** #
# VARIABLES


NAME				:= ex00

CXX_C				:= c++
CXX_FLAGS			:= -Wall -Wextra -Werror -std=c++98 -pedantic

BIN_DIR				:= bin


# **************************************************************************** #
# SOURCES


SRC					:= \
					main.cpp \
					

BIN					:= \
					$(addprefix $(BIN_DIR)/, \
					$(SRC:.cpp=.o))


# **************************************************************************** #
# LIBRARIES & FRAMEWORKS





# **************************************************************************** #
# INCLUDES





# **************************************************************************** #
# RULES


all: $(NAME)

$(NAME): $(BIN)
	$(CXX_C) $(CXX_FLAGS) $(BIN) -o $@

$(BIN_DIR)/%.o: %.cpp
	@mkdir -p $(dir $@)
	$(CXX_C) $(CXX_FLAGS) -c $< -o $@

clean:
	$(RM) -rf $(BIN_DIR)

fclean: clean
	$(RM) -f $(NAME)

re: fclean all


# **************************************************************************** #
# PHONY


.PHONY: all clean fclean re
