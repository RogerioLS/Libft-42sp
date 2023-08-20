
<div align = center>

# Libft-42sp

![42 São Paulo](https://img.shields.io/badge/42-SP-1E2952)
![License](https://img.shields.io/github/license/mendes-jv/libft?color=dark-green)
![Code size in bytes](https://img.shields.io/github/languages/code-size/mendes-jv/libft?color=dark-green)
![Top language](https://img.shields.io/github/languages/top/mendes-jv/libft?color=dark-green)
![Last commit](https://img.shields.io/github/last-commit/mendes-jv/libft?color=dark-green)
</div>

This is the entry project at [École 42](https://www.youtube.com/watch?v=GDHhpy9ANpk&ab_channel=42TheNetwork), in which students are challenged to recreate a set of functions from the classic standardised libC, and other supplementary functions. These functions will then be used throughout the school's curriculum, instead of the standard ones. Students are also welcome to incorporate their own functinos to their libft as needs arrise for the course of the curriculum.

The bonus part of this project comprises functions for the manipulation of singly linked lists.

This project is also the first contact we have with `make` and `Makefile`, and besides the source code for each function and a Makefile, another deliverable is the static library file `libft.a`.

The functions below behave as follows:
Function name | Prototype | Description
:-----------: | :----------- | :-----------
ft_substr | char *ft_substr(const char *s, unsigned int start, size_t len); | Allocates with `malloc` and returns a substring from the string 's', beginning at index 'start' and with maximum size 'len'.
ft_strjoin | char *ft_strjoin(const char *s1, const char *s2); | Allocates with ``malloc`` and returns a new string resulting from the concatenation of strings 's1' and 's2'.
ft_strtrim | char *ft_strtrim(const char *s1, const char *set); | Allocates with `malloc` and returns a copy of the string 's1' with the characters provided in 'set' removed from the beginning and end of the string.
ft_split | char **ft_split(const char *s, char c); | Allocates with `malloc` and returns an array of strings where each word 's' is assigned to each index of the array, with the character 'c' acting as a separator between the words in 's'. The final element of the array is a NULL pointer.
ft_itoa | char *ft_itoa(int n); | Allocates with `malloc` and returns a string representation of the integer received as an argument.
ft_strmapi | char *ft_strmapi(const char *s, char (*f)(unsigned int, char)); | Allocates with `malloc` and returns a string resulting from the application of the function 'f' to each character of the string 's'.
ft_striteri | void ft_striteri(char *s, void (*f)(unsigned int, char*)); | Applies the function 'f' to each index of the string 's'.
ft_putchar_fd | void ft_putchar_fd(char c, int fd); | Outputs the character 'c' to the file descriptor 'fd'.
ft_putstr_fd | void ft_putstr_fd(char *s, int fd); | Outputs the string 's' to the file descriptor 'fd'.
ft_putendl_fd | void ft_putendl_fd(char *s, int fd); | Outputs the string 's' to the file descriptor 'fd', followed by a newline.
ft_putnbr_fd | void ft_putnbr_fd(int n, int fd); | Outputs the integer 'n' to the file descriptor 'fd'.

The following functions are part of the Bonus section of the project and use the data structure declared in libft.h.
Function name | Prototype | Description
:-----------: | :----------- | :-----------
ft_lstnew | t_list *ft_lstnew(void *content); | Allocates a new node with `malloc` and initializes its member variable 'content' with the value of the parameter 'content'.
ft_lstadd_front | void ft_lstadd_front(t_list **lst, t_list *new); | Adds the node 'new' to the start of the list 'lst'
ft_lstadd_back | void ft_lstadd_back(t_list **lst, t_list *new); | Adds the node 'new' to the end of the list 'lst'
ft_lstsize | int ft_lstsize(t_list *lst); | Returns the total number of nodes in the list 'lst'
ft_lstlast | t_list *ft_lstlast(t_list *lst): | Returns a pointer to the last node of the list.
ft_lstdelone | void ft_lstdelone(t_list *lst, void (*del)(void *)); | Frees the content of the node provided as parameter with the function 'del' and then frees the node itself.
ft_lstclear | void ft_lstclear()t_list **lst, void (*del)(void *); | Frees the content of every node in the list 'lst' with the function 'del', and then frees all the nodes. The pointer to the list is set to NULL.
ft_lstiter | void ft_lstiter(t_list *lst, voif (*f)(void *)); | Applies the function 'f' to the content in each node of the list 'lst'.
ft_lstmap | t_list *ft_lstmap(t_list *lst, void *(*f)(void *), void (*del)(void *)); | Returns a copy of the list 'lst', with the function 'f' applied to the content of each node. Uses the function 'del' to delete the content of a node if necessary.

Finally, the functions listed below are either part of other projects, or were developed in my spare time and later added to this library.
Function name | Prototype | Description
:-----------: | :----------- | :-----------
ft_btox | char *ft_btox(void *ptr, size_t size); | Allocates with ``malloc`` and returns the string hexadecimal representation of the value stored in the memory buffer of size passed as parameter at offset 'ptr'.
ft_print_memory | ft_print_memory(const void *addr, size_t size); | Prints 'size' lines of the memory area pointed to by 'addr', 16 bytes per line. The output is divided into three columns: 1) the address offset, 2) the content of each address, in hexadecimal, 3) the content in printable characters. Non-printable characters are replaced by '.' in the 3rd column. If 'addr' is a ``NULL`` pointer, 'size' lines will be printed with the address offset represented as '0x0000000000000000' and both the hex and printable representations of each address as '.'.
get_next_line | get_next_line(int fd); | Reads a file from its descriptor and returns each individual line. This function is made to be used iteratively, so that each call will always return the next line until the end of file.
ft_uitoa | ft_uitoa(unsigned int n); | Allocates with ``malloc`` and returns a string representation of the unsigned integer received as an argument.
ft_abs | int ft_abs(int nbr) | Returns the absloute value of 'nbr'.
ft_max_i | int ft_max_i(int num_a, int num_b) | Returns the largest value between 'num_a' and 'num_b'.
ft_min_i | int ft_min_i(int num_a, int num_b) | Returns the smallest value between 'num_a' and 'num_b'.
ft_str_is_int | bool ft_str_is_int(char *str) | Returns ``true`` if the string 'str' represents a valid ``int`` value; false if otherwise.
ft_free_split | void ft_free_split(char **split) | Frees heap memory allocated into 'split'.
ft_strreplace | char *ft_strreplace(char *str, int index, int torem, char *torepl) | creates a copy of ``str`` with ``malloc``, where ``torem`` bytes are replaced with the string ``torepl`` at offset ``index``

## Compilation instructions
The Makefile is currently configured to compile all parts of the project with `make all`. \
However, the recipes for each part are segregated, in order to make the addition and/or removal of additional functions more convenient when using libft in other projects.

