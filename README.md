# libft

My first C library — a custom reimplementation of common libc-style functions (plus linked list utilities).

This project was my starting point in low-level C programming and helped me build strong fundamentals in memory management, pointer usage, string manipulation, and reusable library design.

---

## Overview

`libft` is a static C library (`libft.a`) containing reimplemented utility functions similar to the standard C library.  
All functions are exposed through `libft.h` and compiled via the provided `Makefile`.

As my **first major programming project**, `libft` taught me how to:
- Think in C (pointers, memory, undefined behaviour)
- Write functions with clear contracts (inputs / outputs)
- Handle edge cases and defensive programming
- Structure code into a reusable library for future projects

---

## Build

```bash
make

This generates:
libft.a

Bonus (linked list utilities):
make bonus

Clean / rebuild:
make clean
make fclean
make re

Included Functions
Character checks & case conversion

ft_isalpha

ft_isdigit

ft_isalnum

ft_isascii

ft_isprint

ft_toupper

ft_tolower

String utilities

ft_strlen

ft_strlcpy

ft_strlcat

ft_strchr

ft_strrchr

ft_strncmp

ft_strnstr

ft_strdup

Memory utilities

ft_bzero

ft_memset

ft_memcpy

ft_memmove

ft_memchr

ft_memcmp

ft_calloc

Conversions

ft_atoi

ft_itoa

String building & transformation

ft_substr

ft_strjoin

ft_strtrim

ft_split

ft_strmapi

ft_striteri

File descriptor output helpers

ft_putchar_fd

ft_putstr_fd

ft_putendl_fd

ft_putnbr_fd

Bonus: Linked List Utilities

Based on the following structure:
typedef struct s_list
{
    void            *content;
    struct s_list   *next;
}   t_list;
Functions included:

ft_lstnew

ft_lstadd_front

ft_lstsize

ft_lstlast

ft_lstadd_back

ft_lstdelone

ft_lstclear

ft_lstiter

ft_lstmap

Notes

This repository focuses on fundamentals and correctness and was used as a base library for later C projects.

Author

Syed Ahmad
GitHub: https://github.com/AlwIkigai
