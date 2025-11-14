# Coding Agent Test

A simple Java project demonstrating binary search implementation. This repository serves as a test project for coding agents and contains a basic binary search algorithm with educational examples.

## Overview

This project implements a binary search algorithm in Java that searches for a target value in a sorted array. The implementation includes a command-line interface for testing the algorithm with custom inputs.

## Features

- Binary search implementation for sorted integer arrays
- Command-line interface for easy testing
- Simple, educational codebase for learning and testing purposes
- IntelliJ IDEA project configuration included

## Prerequisites

Before running this project, ensure you have the following installed:

- **Java Development Kit (JDK)**: Version 8 or higher (tested with Java 17)
  - Download from [Oracle](https://www.oracle.com/java/technologies/downloads/) or use [OpenJDK](https://openjdk.org/)
- **Java Compiler**: `javac` (included with JDK)

To verify your installation:
```bash
java -version
javac -version
```

## Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/ghc-jetbrains/coding-agent-test.git
   cd coding-agent-test
   ```

2. **Compile the source code**:
   ```bash
   cd src
   javac Main.java
   ```

## Usage

The program accepts command-line arguments where:
- The first N-1 arguments are the sorted array elements
- The last argument is the target value to search for

### Basic Usage

```bash
java Main <array elements> <target value>
```

### Examples

**Example 1**: Search for value 3 in array [1, 2, 3, 4, 5]
```bash
java Main 1 2 3 4 5 3
```
Output:
```
Result index: 2
```

**Example 2**: Search for value 7 in array [1, 2, 3, 4, 5]
```bash
java Main 1 2 3 4 5 7
```
Output:
```
Result index: -1
```

**Example 3**: No arguments provided
```bash
java Main
```
Output:
```
Usage: java Main <array elements> <target value>
Example: java Main 1 2 3 4 5 5
```

### Important Notes

- **Array must be sorted**: The binary search algorithm requires a sorted array to function correctly
- **Integer values only**: All input values must be valid integers
- **Return value**: The program returns the index of the found element (0-based) or -1 if not found

## Project Structure

```
coding-agent-test/
├── src/
│   ├── Main.java       # Main class with binary search implementation
│   └── Main.class      # Compiled Java bytecode
├── .idea/              # IntelliJ IDEA configuration
├── .github/            # GitHub configuration and workflows
├── .gitignore          # Git ignore rules
├── test.iml            # IntelliJ IDEA module file
└── README.md           # This file
```

## Code Structure

The main components of the code are:

- **`binarySearch(int[] arr, int b)`**: Implements the binary search algorithm
  - Parameters:
    - `arr`: Sorted array of integers to search
    - `b`: Target value to find
  - Returns: Index of the target value or -1 if not found

- **`main(String[] args)`**: Entry point that:
  - Validates command-line arguments
  - Parses input array and target value
  - Calls binary search
  - Prints the result

## Algorithm Explanation

The binary search algorithm works by:

1. Starting with two pointers at the beginning (`i`) and end (`j`) of the array
2. Calculating the middle index: `a = i + (j - i) / 2`
3. Comparing the middle element with the target:
   - If equal: Return the index
   - If middle element is less than target: Search right half (`i = a + 1`)
   - If middle element is greater than target: Search left half (`j = a - 1`)
4. Repeat until the element is found or the search space is exhausted

**Time Complexity**: O(log n)  
**Space Complexity**: O(1)

## Development

### Using IntelliJ IDEA

This project includes IntelliJ IDEA configuration files (`.iml` and `.idea/`).

1. Open IntelliJ IDEA
2. Select **File → Open**
3. Navigate to the project directory and click **Open**
4. The project should be automatically configured

### Manual Compilation and Execution

From the project root:

```bash
# Compile
cd src
javac Main.java

# Run
java Main 1 2 3 4 5 3

# Clean compiled files
rm *.class
```

## Testing

To test the implementation with various scenarios:

```bash
# Test with even number of elements
java Main 2 4 6 8 10 6

# Test with odd number of elements
java Main 1 3 5 7 9 11 13 7

# Test edge case: single element (found)
java Main 5 5

# Test edge case: single element (not found)
java Main 5 10

# Test with duplicate values
java Main 1 2 2 3 4 2

# Test with negative numbers
java Main -5 -3 -1 0 2 4 -3
```

## Known Issues

- The code contains a note about a potential bug in the binary search implementation (line 7: "Bug: should")
- The condition `while (i < j)` may not handle all edge cases correctly (should potentially be `i <= j`)

## Contributing

Contributions are welcome! This is a test repository, so feel free to:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/improvement`)
3. Make your changes
4. Commit your changes (`git commit -am 'Add improvement'`)
5. Push to the branch (`git push origin feature/improvement`)
6. Create a Pull Request

### Guidelines

- Maintain code simplicity and readability
- Add comments for complex logic
- Test your changes thoroughly
- Follow Java naming conventions

## License

This project is part of the ghc-jetbrains organization and is intended for testing and educational purposes.

## Support

For questions, issues, or contributions:
- Open an issue in the [GitHub repository](https://github.com/ghc-jetbrains/coding-agent-test/issues)
- Contact the maintainers through GitHub

## Acknowledgments

- Created as a test repository for coding agent development
- Binary search algorithm is a fundamental computer science concept
- Thanks to all contributors and testers

---

**Note**: This is a test repository. The code may contain intentional bugs or simplified implementations for educational and testing purposes.
