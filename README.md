
<div align = center>

# Libft-42sp

![42 São Paulo](https://img.shields.io/badge/42-SP-1E2952)
![License](https://img.shields.io/github/license/mendes-jv/libft?color=dark-green)
![Code size in bytes](https://img.shields.io/github/languages/code-size/mendes-jv/libft?color=dark-green)
![Top language](https://img.shields.io/github/languages/top/mendes-jv/libft?color=dark-green)
![Last commit](https://img.shields.io/github/last-commit/mendes-jv/libft?color=dark-green)
</div>

---

<div align = center>

![](https://game.42sp.org.br/static/assets/achievements/libftm.png)

[![roglopes's 42 Libft Score](https://badge42.vercel.app/api/v2/clljwl4dk005408mn48ta77wy/project/3196037)](https://github.com/JaeSeoKim/badge42)

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

## Compilation instructions
The Makefile is currently configured to compile all parts of the project with `make all`. \
However, the recipes for each part are segregated, in order to make the addition and/or removal of additional functions more convenient when using libft in other projects.

