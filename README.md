# Binary Search Demo

A simple Java application that demonstrates a binary search algorithm implementation. This project is designed for educational purposes and includes a command-line interface for searching values in sorted arrays.

## Features

- Command-line binary search implementation
- Accepts arrays and target values as command-line arguments
- Returns the index of the found element or -1 if not found
- Simple and easy-to-understand code structure

## Requirements

- Java Development Kit (JDK) 8 or higher
- A Java IDE (recommended: IntelliJ IDEA) or command-line tools

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/ghc-jetbrains/coding-agent-test.git
   cd coding-agent-test
   ```

2. Compile the Java source file:
   ```bash
   javac src/Main.java
   ```

## Usage

Run the application from the command line with the following syntax:

```bash
java -cp src Main <array elements> <target value>
```

### Examples

Search for the value 5 in the array [1, 2, 3, 4, 5]:
```bash
java -cp src Main 1 2 3 4 5 5
```

Search for the value 10 in the array [2, 4, 6, 8]:
```bash
java -cp src Main 2 4 6 8 10
```

### Usage Notes

- The array elements should be sorted in ascending order for binary search to work correctly
- All array elements and the target value should be integers
- The last argument is treated as the target value to search for
- The program will output the index of the target value in the array, or -1 if not found

## Project Structure

```
coding-agent-test/
├── .github/           # GitHub configurations
├── .idea/             # IntelliJ IDEA project files
├── src/
│   └── Main.java      # Main application with binary search implementation
├── .gitignore         # Git ignore rules
├── test.iml           # IntelliJ IDEA module file
└── README.md          # This file
```

## Known Issues

⚠️ **Note**: The current binary search implementation contains a known bug in the loop condition (line 7: `while (i < j)` should be `while (i <= j)`). This may cause the search to fail in certain edge cases, particularly when searching for the last element in the array.

## Contributing

Contributions are welcome! If you'd like to fix the binary search bug or improve the code:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/improvement`)
3. Make your changes
4. Commit your changes (`git commit -am 'Add improvement'`)
5. Push to the branch (`git push origin feature/improvement`)
6. Open a Pull Request

## License

This project is provided as-is for educational purposes.
