# coding-agent-test

A simple Java project demonstrating a binary search algorithm.

## Overview

This project contains a `Main` class that implements binary search on a sorted integer array.
It accepts an array of integers and a target value as command-line arguments, then prints the
index of the target value in the array, or `-1` if the target is not found.

## Requirements

- Java 8 or later

## Building

Compile the source file from the repository root:

```bash
javac src/Main.java -d out
```

## Usage

Run the compiled class, providing the sorted array elements followed by the target value as arguments:

```bash
java -cp out Main <array elements> <target value>
```

### Examples

Search for `3` in the array `[1, 2, 3, 4, 5]`:

```bash
java -cp out Main 1 2 3 4 5 3
# Result index: 2
```

Search for a value that does not exist:

```bash
java -cp out Main 1 2 3 4 5 9
# Result index: -1
```

## Project Structure

```
src/
  Main.java   # Binary search implementation and entry point
```
