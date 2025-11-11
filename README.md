# Coding Agent Test

A simple Java project demonstrating a binary search algorithm implementation for testing purposes.

## Description

This project contains a Java implementation of the binary search algorithm. It's designed as a test project to demonstrate basic Java programming concepts and algorithm implementation.

## Features

- Binary search algorithm implementation
- Command-line interface for testing the algorithm
- Support for integer arrays and target value searching

## Prerequisites

- Java Development Kit (JDK) 8 or higher
- A Java-compatible IDE (IntelliJ IDEA, Eclipse, etc.) or command-line Java compiler

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/ghc-jetbrains/coding-agent-test.git
   cd coding-agent-test
   ```

2. Compile the Java source files:
   ```bash
   javac src/Main.java -d out
   ```

## Usage

Run the program from the command line with the following syntax:

```bash
java -cp out Main <array elements> <target value>
```

### Examples

Search for the value `5` in the array `[1, 2, 3, 4, 5]`:
```bash
java -cp out Main 1 2 3 4 5 5
```

Search for the value `3` in the array `[1, 2, 3, 4, 5, 6, 7, 8, 9, 10]`:
```bash
java -cp out Main 1 2 3 4 5 6 7 8 9 10 3
```

### Output

The program will output the index of the target value in the array, or `-1` if the value is not found:
```
Result index: 2
```

## Project Structure

```
coding-agent-test/
├── src/
│   └── Main.java          # Main class with binary search implementation
├── .gitignore             # Git ignore file
├── test.iml               # IntelliJ IDEA module file
└── README.md              # This file
```

## Binary Search Implementation

The project includes a `binarySearch` method that:
- Takes a sorted integer array and a target value as input
- Returns the index of the target value if found
- Returns -1 if the target value is not present in the array

## License

This is a test project. Please refer to the repository owner for licensing information.

## Contributing

This is a test repository. For contributions or questions, please contact the repository maintainers.
