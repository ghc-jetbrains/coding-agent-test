# Coding Agent Test

A Java project demonstrating a binary search algorithm implementation.

## Overview

This project contains a simple Java application that implements binary search functionality. The `Main` class provides a binary search method to find elements in a sorted integer array.

## Features

- Binary search algorithm implementation
- Command-line interface for searching arrays
- Simple usage pattern with array elements and target value

## Requirements

- Java Development Kit (JDK) 8 or higher
- IntelliJ IDEA (optional, project files included)

## Installation

1. Clone the repository:
```bash
git clone https://github.com/ghc-jetbrains/coding-agent-test.git
cd coding-agent-test
```

2. Compile the source code:
```bash
javac src/Main.java
```

## Usage

Run the program with an array of integers followed by the target value to search for:

```bash
java -cp src Main <array elements> <target value>
```

### Example

```bash
java -cp src Main 1 2 3 4 5 5
```

This will search for the value `5` in the array `[1, 2, 3, 4, 5]`.

### Output

The program will output the index of the target element in the array, or `-1` if the element is not found:

```
Result index: 4
```

## Project Structure

```
.
├── src/
│   └── Main.java          # Main application with binary search implementation
├── .gitignore             # Git ignore file
├── test.iml               # IntelliJ IDEA module file
└── README.md              # This file
```

## Development

This project is set up as an IntelliJ IDEA module. You can:

1. Open the project in IntelliJ IDEA
2. Navigate to `src/Main.java`
3. Run the application using the IDE's run configuration

## License

This project is for testing and educational purposes.
