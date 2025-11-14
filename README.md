# Coding Agent Test

A simple Java project containing a binary search implementation for testing and educational purposes. This repository is part of the ghc-jetbrains organization and serves as a test project for coding agents and development workflows.

## Overview

This project implements a binary search algorithm in Java with an intentional bug to demonstrate debugging and testing scenarios. It's designed to be a straightforward example for:
- Testing automated coding agents
- Learning about binary search algorithms
- Practicing debugging skills
- Understanding common algorithmic pitfalls

## Features

- Binary search implementation in Java
- Command-line interface for easy testing
- Simple array searching functionality
- Educational bug demonstration

## Prerequisites

- Java Development Kit (JDK) 8 or higher
- Basic understanding of Java and command-line operations

## Installation

1. Clone the repository:
```bash
git clone https://github.com/ghc-jetbrains/coding-agent-test.git
cd coding-agent-test
```

2. Compile the Java source file:
```bash
cd src
javac Main.java
```

## Usage

Run the program with an array of integers followed by the target value to search for:

```bash
java Main <array elements> <target value>
```

### Example

```bash
java Main 1 2 3 4 5 5
```

This searches for the value `5` in the array `[1, 2, 3, 4, 5]`.

### Output

The program will output:
```
Result index: <index>
```

Where `<index>` is:
- The position of the target element in the array (0-indexed), or
- `-1` if the element is not found

### Help

Running the program without arguments displays usage information:
```bash
java Main
```

## Project Structure

```
coding-agent-test/
├── .github/          # GitHub configuration
├── .idea/            # IntelliJ IDEA project files
├── src/
│   └── Main.java     # Main source file with binary search implementation
├── .gitignore        # Git ignore rules
├── test.iml          # IntelliJ IDEA module file
└── README.md         # This file
```

## Known Issues

⚠️ **Intentional Bug**: The binary search implementation contains a known bug on line 7. The loop condition uses `i < j` instead of `i <= j`, which may cause the algorithm to miss the target value in certain cases. This is intentional for educational and testing purposes.

## Development

This project uses IntelliJ IDEA as the primary IDE, but can be developed with any Java IDE or text editor.

### Building

To compile the source code:
```bash
javac src/Main.java
```

The compiled `.class` files will be generated in the `src` directory and are excluded from version control via `.gitignore`.

## Contributing

This is a test repository for the ghc-jetbrains organization. If you'd like to contribute:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/your-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin feature/your-feature`)
5. Create a Pull Request

## License

This project is part of the ghc-jetbrains organization test suite. Please refer to the organization's licensing policies.

## Support

For issues, questions, or contributions, please use the GitHub issue tracker for this repository.
