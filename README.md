# Coding Agent Test

A Java project demonstrating a binary search implementation for testing and educational purposes.

## Description

This project contains a simple Java program that implements a binary search algorithm. The program accepts an array of integers and a target value as command-line arguments, then searches for the target value in the array using binary search.

## Features

- Binary search implementation for integer arrays
- Command-line interface for easy testing
- Returns the index of the target element or -1 if not found

## Requirements

- Java Development Kit (JDK) 8 or higher
- A Java-compatible IDE (IntelliJ IDEA recommended) or command-line tools

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/ghc-jetbrains/coding-agent-test.git
   cd coding-agent-test
   ```

2. Compile the Java source code:
   ```bash
   javac src/Main.java
   ```

## Usage

Run the program from the command line with the following syntax:

```bash
java -cp src Main <array elements> <target value>
```

### Example

```bash
java -cp src Main 1 2 3 4 5 5
```

This command searches for the value `5` in the array `[1, 2, 3, 4, 5]`.

### Output

The program outputs the index of the target value if found, or `-1` if not found:

```
Result index: 4
```

## Project Structure

```
coding-agent-test/
├── src/
│   └── Main.java          # Main program with binary search implementation
├── .gitignore             # Git ignore rules
├── .idea/                 # IntelliJ IDEA project configuration
├── test.iml               # IntelliJ IDEA module file
└── README.md              # This file
```

## How It Works

The binary search algorithm:
1. Takes a sorted array and a target value as input
2. Repeatedly divides the search interval in half
3. Compares the middle element with the target
4. Adjusts the search boundaries based on the comparison
5. Returns the index when found, or -1 if the target is not in the array

## Development

### Using IntelliJ IDEA

1. Open the project in IntelliJ IDEA
2. Navigate to `src/Main.java`
3. Press the Run button or use the shortcut to execute the program
4. Configure run arguments in the Run Configuration dialog

### Command Line

Compile and run from the terminal as shown in the Usage section above.

## Contributing

Contributions are welcome! Please feel free to submit issues or pull requests.

## License

This project is available for educational and testing purposes.
