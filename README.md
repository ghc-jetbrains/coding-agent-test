# Coding Agent Test

A simple Java test repository containing a binary search implementation, used for testing and demonstrating coding agent capabilities.

## Description

This repository contains a minimal Java project with a `Main` class that implements a binary search algorithm. The project is designed to serve as a test case for coding agents and automated code analysis tools.

## Project Structure

```
.
├── src/
│   └── Main.java       # Main class with binary search implementation
├── .idea/              # IntelliJ IDEA project files
├── test.iml            # IntelliJ IDEA module file
└── README.md           # This file
```

## Requirements

- Java Development Kit (JDK) 8 or higher
- (Optional) IntelliJ IDEA for IDE support

## Building and Running

### Compile the Code

```bash
javac src/Main.java
```

### Run the Program

The program accepts an array of integers followed by a target value to search for:

```bash
java -cp src Main <array elements> <target value>
```

#### Example

```bash
java -cp src Main 1 2 3 4 5 5
```

This will search for the value `5` in the array `[1, 2, 3, 4, 5]` and print the index where it's found (or `-1` if not found).

### Usage Help

Running the program without arguments displays usage information:

```bash
java -cp src Main
```

Output:
```
Usage: java Main <array elements> <target value>
Example: java Main 1 2 3 4 5 5
```

## Features

- Binary search algorithm implementation
- Command-line interface for testing
- Simple structure for educational purposes

## Development

This project uses IntelliJ IDEA as the primary IDE. The `.iml` and `.idea` configuration files are included for convenience.

### Opening in IntelliJ IDEA

1. Open IntelliJ IDEA
2. Select "Open" from the welcome screen
3. Navigate to the project directory and select it
4. IntelliJ will recognize the project structure automatically

## Notes

The binary search implementation in this repository may contain intentional bugs or issues for testing purposes. This is a test repository and should be used for demonstration and testing only.

## License

This is a test repository. Please check with the repository maintainers for licensing information.
