# Coding Agent Test

A simple Java project demonstrating a binary search implementation.

## Description

This project contains a Java implementation of a binary search algorithm. It serves as a test project for coding agents and demonstrates basic Java programming concepts.

## Prerequisites

- Java Development Kit (JDK) 8 or higher
- A Java IDE (IntelliJ IDEA recommended) or command-line Java compiler

## Project Structure

```
coding-agent-test/
├── src/
│   └── Main.java          # Main class with binary search implementation
├── .gitignore             # Git ignore rules
├── test.iml               # IntelliJ IDEA module file
└── README.md              # This file
```

## Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/ghc-jetbrains/coding-agent-test.git
   cd coding-agent-test
   ```

2. Compile the Java source file:
   ```bash
   javac src/Main.java
   ```

## Usage

Run the program with a sorted array of integers followed by a target value to search for:

```bash
java -cp src Main <array elements> <target value>
```

### Examples

Search for value 5 in array [1, 2, 3, 4, 5]:
```bash
java -cp src Main 1 2 3 4 5 5
```

Search for value 3 in array [1, 2, 3, 4, 5]:
```bash
java -cp src Main 1 2 3 4 5 3
```

The program will output the index of the target value in the array, or -1 if not found.

## Features

- Binary search implementation
- Command-line interface
- Input validation and usage instructions

## Development

### Opening in IntelliJ IDEA

1. Open IntelliJ IDEA
2. Select "Open" and navigate to the project directory
3. The project should be recognized automatically through the `test.iml` file

### Compiling and Running in IDE

- Right-click on `Main.java` and select "Run 'Main.main()'"
- Configure run arguments in the run configuration settings

## License

This project is available for educational and testing purposes.

## Contributing

This is a test project for coding agents. Contributions can be made through pull requests.
