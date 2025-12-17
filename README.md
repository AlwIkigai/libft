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
```

This generates:
```txt
libft.a
```

### Bonus (linked list utilities):
```bash
make bonus
```

### Clean / rebuild:
```bash
make clean
make fclean
make re
```

## Included Functions

### Character checks & case conversion
- **ft_isalpha** – checks whether a character is alphabetic
- **ft_isdigit** – checks whether a character is a digit
- **ft_isalnum** – checks whether a character is alphanumeric
- **ft_isascii** – checks whether a character is a valid ASCII value
- **ft_isprint** – checks whether a character is printable
- **ft_toupper** – converts a lowercase character to uppercase
- **ft_tolower** – converts an uppercase character to lowercase


### String utilities

- **ft_strlen** – returns the length of a string
- **ft_strlcpy** – copies a string with size limitation
- **ft_strlcat** – concatenates strings with size limitation
- **ft_strchr** – locates the first occurrence of a character in a string
- **ft_strrchr** – locates the last occurrence of a character in a string
- **ft_strncmp** – compares two strings up to a given length
- **ft_strnstr** – locates a substring within a string up to a given length
- **ft_strdup** – duplicates a string into newly allocated memory


### Memory utilities

- **ft_bzero** – sets a block of memory to zero
- **ft_memset** – fills a block of memory with a specified byte value
- **ft_memcpy** – copies memory from source to destination
- **ft_memmove** – copies memory safely, handling overlapping regions
- **ft_memchr** – locates a byte in a block of memory
- **ft_memcmp** – compares two blocks of memory
- **ft_calloc** – allocates and zero-initializes memory


### Conversions

- **ft_atoi** – converts a string to an integer
- **ft_itoa** – converts an integer to a string


### String building & transformation

- **ft_substr** – extracts a substring from a string
- **ft_strjoin** – concatenates two strings into a new string
- **ft_strtrim** – trims specified characters from the start and end of a string
- **ft_split** – splits a string into an array using a delimiter
- **ft_strmapi** – applies a function to each character of a string and returns a new string
- **ft_striteri** – applies a function to each character of a string in place


### File descriptor output helpers

- **ft_putchar_fd** – writes a character to a file descriptor
- **ft_putstr_fd** – writes a string to a file descriptor
- **ft_putendl_fd** – writes a string followed by a newline to a file descriptor
- **ft_putnbr_fd** – writes an integer to a file descriptor

### Bonus: Linked List Utilities

Based on the following structure:
```c
typedef struct s_list
{
    void            *content;
    struct s_list   *next;
}   t_list;
```
###  Functions included:

- **ft_lstnew** – creates a new list node
- **ft_lstadd_front** – adds a node at the beginning of a list
- **ft_lstsize** – returns the number of nodes in a list
- **ft_lstlast** – returns the last node of a list
- **ft_lstadd_back** – adds a node at the end of a list
- **ft_lstdelone** – deletes a single list node
- **ft_lstclear** – deletes and frees an entire list
- **ft_lstiter** – applies a function to each node’s content
- **ft_lstmap** – creates a new list by applying a function to each node


##  Notes

This repository focuses on fundamentals and correctness and was used as a base library for later C projects.

##  Author

Syed Ahmad
GitHub: https://github.com/AlwIkigai
