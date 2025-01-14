# SongAnalyzer-C

Assignment 3 for SENG265: Software Development Methods at UVic

A C program that analyzes song data using linked list data structures to process and organize music information.

See the python version [here](https://github.com/n4m3name/SongAnalyzer-Py)

## Core Features

- Dynamic linked list implementation for song data storage
- Word frequency analysis
- Custom memory management
- Thread-safe operations
- Ordered list manipulation

## Technical Implementation

**Main Components**
```c
node_t *list = NULL;
char *line = NULL;
line = (char *)malloc(sizeof(char) * MAX_LINE_LEN);
```

**Key Functions**
- `analysis()`: Performs word count and content analysis
- `inccounter()`: Incremental counter for list navigation
- `print_node()`: Displays node content
- `add_inorder()`: Maintains sorted list structure

## Memory Management

- Safe memory allocation through `emalloc` wrapper
- Proper cleanup of allocated resources
- NULL pointer validation
- Dynamic string handling

## Usage

1. Compile the program:
```bash
gcc -o song_analyzer song_analyzer.c list.c emalloc.c -Wall
```

2. Run with input:
```bash
./song_analyzer < input.txt
```

## Dependencies

- Standard C libraries
- POSIX-compliant system
- Custom list implementation
- Memory allocation wrapper

## Project Structure

- `song_analyzer.c`: Main program logic
- `list.c`: Linked list implementation
- `list.h`: List interface declarations
- `emalloc.c`: Memory management wrapper
- `emalloc.h`: Memory allocation interface

## Authors

- Mike Z.
- Felipe R.
- Hausi M.
- Juan G.
- Angadh S.
- Evan S.
