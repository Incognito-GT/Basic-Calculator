# Java Calculator

A simple command-line calculator application written in Java that performs basic arithmetic operations.

## Features

- Addition (+)
- Subtraction (-)
- Multiplication (*)
- Division (/)
- Clean command-line interface
- Input validation
- Continuous operation until user chooses to exit

## Prerequisites

- Java Development Kit (JDK) 11 or later
- Maven (optional, for building with dependencies)

## Getting Started

### Installation

1. Clone the repository or download the source code
2. Navigate to the project directory:
   ```bash
   cd java-calculator
   ```

### Running the Application

#### Option 1: Using Maven (Recommended)
```bash
mvn clean package
exec:java
```

#### Option 2: Direct Java Execution
```bash
# Compile the code
javac src/main/java/com/calculator/Calculator.java -d target/classes

# Run the application
java -cp target/classes com.calculator.Calculator
```

## How to Use

1. Run the program using one of the methods above
2. You'll see a menu with the following options:
   - 1. Add (+)
   - 2. Subtract (-)
   - 3. Multiply (*)
   - 4. Divide (/)
   - 5. Exit
3. Enter your choice (1-5)
4. For operations 1-4, you'll be prompted to enter two numbers
5. The result will be displayed
6. The program will continue until you choose option 5 to exit

## Example

```
Simple Calculator
-----------------
Operations:
1. Add (+)
2. Subtract (-)
3. Multiply (*)
4. Divide (/)
5. Exit

Enter your choice (1-5): 1
Enter first number: 5
Enter second number: 3

Result: 5.00 + 3.00 = 8.00
```

## Error Handling

- Division by zero is handled with an appropriate error message
- Invalid menu choices are caught and the user is prompted again
- Non-numeric inputs are handled gracefully

## Project Structure

```
java-calculator/
├── src/
│   └── main/
│       └── java/
│           └── com/
│               └── calculator/
│                   └── Calculator.java
├── target/
│   └── classes/    # Compiled .class files
├── pom.xml         # Maven configuration
└── README.md       # This file
```
