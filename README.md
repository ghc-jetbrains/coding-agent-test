# Coding Agent Test

A simple Java project containing a binary search implementation, designed for testing coding agents and automated code analysis tools.

## Description

This repository contains a basic Java application that implements a binary search algorithm. The implementation includes an intentional bug for testing purposes, making it useful for:
- Testing coding agents
- Demonstrating bug detection capabilities
- Educational purposes
- Code review practice

## Project Structure

```
.
├── src/
│   └── Main.java       # Main class with binary search implementation
├── .gitignore          # Git ignore patterns
├── test.iml            # IntelliJ IDEA module file
└── README.md           # This file
```

## Requirements

- Java Development Kit (JDK) 8 or higher
- A Java compiler (`javac`)

## Compilation

To compile the project, navigate to the project root directory and run:

```bash
javac src/Main.java
```

This will generate `Main.class` in the `src` directory.

## Usage

The program performs a binary search on an array of integers to find a target value.

### Syntax

```bash
java -cp src Main <array elements> <target value>
```

### Parameters

- `<array elements>`: Space-separated integers representing the sorted array
- `<target value>`: The integer to search for in the array

### Examples

```bash
# Search for 5 in the array [1, 2, 3, 4, 5]
java -cp src Main 1 2 3 4 5 5

# Search for 3 in the array [1, 2, 3, 4, 5, 6, 7, 8, 9]
java -cp src Main 1 2 3 4 5 6 7 8 9 3

# Search for 10 in the array [1, 2, 3, 4, 5]
java -cp src Main 1 2 3 4 5 10
```

### Expected Output

The program outputs the index of the target value in the array (0-indexed), or `-1` if the value is not found.

Example output:
```
Result index: 4
```

## Known Issues

The binary search implementation contains a known bug in the while loop condition (line 7). This is intentional and serves as a test case for code analysis tools.

## Contributing

This is a test repository for coding agents. Feel free to fork and experiment with it.

## License

This project is available for educational and testing purposes.
