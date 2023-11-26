<div align = center>

# :books: Libft | 42 SP

[![Norminette and Build](https://github.com/RogerioLS/Libft-42sp/actions/workflows/main.yml/badge.svg)](https://github.com/RogerioLS/Libft-42sp/actions/workflows/main.yml)
![Static Badge](https://img.shields.io/badge/LIBFT-42-blue)
![42 São Paulo](https://img.shields.io/badge/42-SP-1E2952)
![License](https://img.shields.io/github/license/RogerioLS/Libft-42sp?color=dark-green)
![Code size in bytes](https://img.shields.io/github/languages/code-size/RogerioLS/Libft-42sp?color=dark-green)
![Top language](https://img.shields.io/github/languages/top/RogerioLS/Libft-42sp?color=dark-green)
![Last commit](https://img.shields.io/github/last-commit/RogerioLS/Libft-42sp?color=dark-green)
![Repo size](https://img.shields.io/github/repo-size/RogerioLS/Libft-42sp)
![Languages](https://img.shields.io/github/languages/count/RogerioLS/Libft-42sp?color=red)
![Lines Of Code](https://tokei.rs/b1/github/RogerioLS/Libft-42sp?category=code)
![Discord](https://img.shields.io/discord/1114673462859006044?label=testemunhas%20de%20vim&color=ffbe3a)

</div>

---

<div align = center>

![](https://game.42sp.org.br/static/assets/achievements/libftm.png)

[![roglopes's 42 Libft Score](https://badge42.vercel.app/api/v2/clljwl4dk005408mn48ta77wy/project/3196037)](https://github.com/JaeSeoKim/badge42)
</div>

- Actual Status : finished.
- Result        : evaluation in progress.

The libft (42 Library) is the first project in the software engineering curriculum at 42 São Paulo. The objective of the project is to create your first C library by re-creating functions from the standard C library. During the project, you will learn how these functions work, how to implement them, and how to use each one. To submit the project, you must create a Makefile that compiles your library without relinking.

Upon completing the mandatory part of the project, you are encouraged to do the bonus part, which involves learning about linked lists, how to create them, and how to manipulate them.

## 📝 Functions

| Function | Description |
| :------: | :---------: |
| ``ft_atoi`` | Converts the initial portion of the string pointed to by ``nptr`` to int. |
| ``ft_bzero`` | Sets the first ``n`` chars of a string ``s`` to zero ``\0``. |
| ``ft_calloc`` | Allocates memory for an array of 'nmemb' elements of 'size' bytes, and set to zero. |
| ``ft_isalnum`` | Returns ``1`` if the input is a alphanumeric character from the ``ASCII`` table. |
| ``ft_isalpha`` | Returns ``1`` if the input is a alphabetical character from the ``ASCII`` table. |
| ``ft_isascii`` | Returns ``1`` if the input is in the ``ASCII`` table. |
| ``ft_isdigit`` | Returns ``1`` if the input is a digit character from the ``ASCII`` table. |
| ``ft_isprint`` | Returns ``1`` if the input is a printable character from the ``ASCII`` table. |
| ``ft_itoa`` | Allocates with malloc and returns a string representing the integer received as an argument, negative numbers must be handled. |
| ``ft_memccpy`` | Copies from one memory point to another, until the specified character is copied or until ``n`` bytes are copied. |
| ``ft_memchr`` | Scans the initial ``n`` bytes of the memory area pointed to by ``s`` for the first instance of ``c``. |
| ``ft_memcmp`` | Compares the first ``n`` bytes, each interpreted as unsigned char, of the memory areas ``s1`` and ``s2``. |
| ``ft_memcpy`` | Copies ``n`` bytes from memory area ``src`` to memory area ``dest``, the memory areas must not overlap. |
| ``ft_memmove`` | Copies ``n`` bytes from memory area ``src`` to memory area ``dest``, cases of memory overlap must be handled. |
| ``ft_memset`` | Fills the first ``n`` bytes of the memory area pointed to by ``s`` with the int ``c``. |
| ``ft_putchar_fd`` | Outputs the character ``c`` to the given file descriptor. |
| ``ft_putendl_fd`` | Outputs the string ``s`` to the given file descriptor followed by a newline. |
| ``ft_putnbr_fd`` | Outputs the integer ``n`` to the given file descriptor. |
| ``ft_putstr_fd`` | Outputs the string ``s`` to the given file descriptor. |
| ``ft_split`` | Allocates with malloc and returns an array of strings obtained by splitting ``s`` using the character ``c`` as a delimiter. |
| ``ft_strchr`` | Looks for the first occurrence of the character ``c`` in the string ``s``. |
| ``ft_strdup`` | Allocates with malloc and duplicate the contents of string ``s``. |
| ``ft_striteri`` | Applies the function ``f`` on each character of the string passed as argument. |
| ``ft_strjoin`` | Allocates with malloc and returns a new string, which is the result of the concatenation of ``s1`` and ``s2``. |
| ``ft_strlcat`` | Appends the NUL-terminated string ``src`` to the end of ``dst``. |
| ``ft_strlcpy`` | Copies ``size - 1`` characters from the NUL-terminated string ``src`` to ``dst``, NUL-terminating the result. |
| ``ft_strlen`` | Returns the length of the string, before the terminating null byte ``\0`` can be found. |
| ``ft_strmapi`` | Create a new string with malloc resulting from successive applications of ``f``. |
| ``ft_strncmp`` | Compares only the first (at most) n bytes of two strings, ``s1`` and ``s2``. |
| ``ft_strnstr`` | Locates the first occurrence of the null-terminated string ``little`` in the string ``big``, where not more than ``len`` characters are searched. Characters that appear after a ``\0`` are not searched. |
| ``ft_strrchr`` | Looks for the last occurrence of the character ``c`` in the string ``s``. |
| ``ft_strtrim`` | Allocates with malloc and returns a copy of ``s1`` with the characters specified in ``set`` removed from the beginning and the end of the string. |
| ``ft_substr`` | Allocates with malloc and returns a substring from the string ``s``. The substring begins at index ``start`` and is of maximum size ``len``. |
| ``ft_tolower`` | Convert uppercase letters to lowercase. |
| ``ft_toupper`` | Convert lowercase letters to uppercase. |

## :star: Bonus
For this part we implemented a struct defining the well-known linked lists
```C
typedef	struct	s_list
{
	void		*content;
	struct	s_list	*next;
}			t_list;
```

Bonus functions to implement

| Bonus Function | Description |
| :------------: | :---------: |
| ``ft_lstnew`` | Allocates with malloc and returns a new node. |
| ``ft_lstadd_front`` | Adds the node ``new`` at the beginning of the list. |
| ``ft_lstsize`` | Counts the number of nodes in a list. |
| ``ft_lstlast`` | Returns the last node of the list. |
| ``ft_lstadd_back`` | Adds the node ``new`` at the end of the list. |
| ``ft_lstdelone`` | Takes as a parameter a node and frees the memory of the node’s content. The memory of ``next`` must not be freed. |
| ``ft_lstclear`` | Deletes and frees the given node and every successor of that node and set the pointer to the list with NULL. |
| ``ft_lstiter`` | Iterates the list ``lst`` and applies the function ``f`` on the content of each node. |
| ``ft_lstmap`` | Creates a new list resulting of the successive applications of the function ``f``. Use ``del`` if you need to delete the content. |

## 🛠️ Usage

## Compilation instructions
The Makefile is currently configured to compile all parts of the project with `make all`. \
However, the recipes for each part are segregated, in order to make the addition and/or removal of additional functions more convenient when using libft in other projects.

## How to use

Clone this repository:
```shell
$ git clone https://github.com/RogerioLS/Libft-42sp.git
```

Run `make` on it:
```shell
$ make
```

If you want to use linked lists, run `make bonus`:
```shell
$ make bonus
```

Include `libft.h` in your `.c`:
```c
#include "../include/libft.h"
```

Compile your `.c` with the library:
```shell
$ cc my_program.c libft.a
```

