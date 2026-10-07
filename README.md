# Customised Virtual File System (CVFS)

A custom virtual file system implemented in C that simulates basic file system operations in memory. The project demonstrates how file systems manage files, metadata, permissions, file descriptors, and storage structures.

## Features

- Custom shell interface for interacting with the virtual file system
- File creation and deletion
- File reading and writing
- File listing and metadata display
- File permission management
- File descriptor and offset management
- Custom `help` and `man` commands
- In-memory file system implementation
- Error handling for invalid file operations

## Technologies Used

- C
- Linux/UNIX System Programming
- Data Structures
- File System Concepts
- Pointers and Dynamic Memory Allocation

## File System Architecture

The CVFS is organized using different internal structures to manage files and their metadata:

```text
CVFS
 │
 ├── BootBlock
 │
 ├── SuperBlock
 │
 ├── DILB
 │    └── Inode Information
 │
 ├── UAREA
 │    └── Open File Table
 │
 └── File Data
