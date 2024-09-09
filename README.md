
#  Femto Unix Utilities

This repository contains custom implementations of common Unix-like utilities in C. These utilities mimic the behavior of their standard counterparts (`cp`, `echo`, `mv`, and `pwd`) but with simplified logic and structure.

## Programs

### 1. `mycp.c`
This program is a custom implementation of the Unix `cp` command. It copies files from one location to another.
![mycpy](https://github.com/user-attachments/assets/422c6c66-d17e-4a4b-a425-54596b237e1d)

#### Usage:
```bash
./mycp source_file destination_file
```

#### Features:
- Copies the contents of the `source_file` to the `destination_file`.
- Supports basic file error handling.

### 2. `myecho.c`
This program is a custom implementation of the Unix `echo` command. It outputs the arguments provided to it.
![echo](https://github.com/user-attachments/assets/0ee147e1-7393-499e-a994-97e3f7bc5194)

#### Usage:
```bash
./myecho [arguments...]
```

#### Features:
- Prints the given arguments to the standard output.
- Supports multiple arguments and handles them as the standard `echo` does.

### 3. `mymv.c`
This program is a custom implementation of the Unix `mv` command. It moves or renames files.
![mymv](https://github.com/user-attachments/assets/897abd9f-5915-4465-b7a5-f26765d58e95)

#### Usage:
```bash
./mymv source_file destination_file
```

#### Features:
- Moves or renames the `source_file` to `destination_file`.
- Includes basic file handling for renaming and moving.

### 4. `mypwd.c`
This program is a custom implementation of the Unix `pwd` command. It prints the current working directory using the `getcwd()` function.
![mypwd](https://github.com/user-attachments/assets/374ababc-23ed-4b3e-b9c8-d7289bfd3525)

#### Usage:
```bash
./mypwd
```

#### Features:
- Retrieves and prints the current working directory using `getcwd()`.
- Handles errors if the path exceeds `PATH_MAX`.

## Compilation
To compile these programs, use the following commands:

```bash
gcc -o mycp mycp.c
gcc -o myecho myecho.c
gcc -o mymv mymv.c
gcc -o mypwd mypwd.c
```

## Notes
- These programs are basic implementations and do not include all advanced features of the original Unix utilities.
- The `mypwd.c` program demonstrates how to retrieve and display the current working directory.
- They are designed for educational purposes or simple use cases.

## License
This project is licensed under the MIT License - see the LICENSE file for details.
