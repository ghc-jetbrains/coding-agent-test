# Binary Search Demo

A simple Java application that demonstrates binary search algorithm implementation.

## Description

This project contains a Java implementation of the binary search algorithm. The program searches for a target value in a sorted array of integers and returns the index of the target value if found, or -1 if not found.

## Features

- Binary search implementation
- Command-line interface for testing
- Handles arrays of integers

## Requirements

- Java Development Kit (JDK) 8 or higher
- A Java compiler (javac)

## Compilation

To compile the program, navigate to the project root directory and run:

```bash
javac src/Main.java
```

This will generate the compiled class file in the `src` directory.

## Usage

Run the program from the project root directory using:

```bash
java -cp src Main <array elements> <target value>
```

### Command-line Arguments

- `<array elements>`: Space-separated integers representing the sorted array
- `<target value>`: The integer value to search for in the array

### Example

```bash
java -cp src Main 1 2 3 4 5 5
```

This searches for the value `5` in the array `[1, 2, 3, 4, 5]`.

### Output

The program will print the index of the target value if found, or -1 if the value is not in the array:

```
Result index: 4
```

## Notes

- The input array should be sorted for binary search to work correctly
- Array indices are zero-based
- If the array is not sorted, results may be incorrect

## Project Structure

```
.
├── README.md           # This file
├── src/
│   └── Main.java      # Main application with binary search implementation
├── .gitignore         # Git ignore rules
└── test.iml           # IntelliJ IDEA project file
```

## Development

This project can be opened in IntelliJ IDEA or any other Java IDE. The `.iml` file contains the IntelliJ IDEA project configuration.

## License

This is a demo project for educational purposes.
