# Calculator
#Scientific Calculator
#include <iostream>
#include <cmath>

// Addition
int add(int x, int y) {
    int sum = x + y;
    std::cout << "The sum is: " << sum << std::endl;
    return sum;
}

// Subtraction
int subtract(int x, int y) {
    int difference = x - y;
    std::cout << "The difference is: " << difference << std::endl;
    return difference;
}

// Multiplication
int multiply(int x, int y) {
    int product = x * y;
    std::cout << "The product is: " << product << std::endl;
    return product;
}

// Division
double divide(int x, int y) {
    if (y == 0) {
        std::cout << "Error: Division by zero is not allowed." << std::endl;
        return 0.0;
    }
    double quotient = static_cast<double>(x) / y;
    std::cout << "The quotient is: " << quotient << std::endl;
    return quotient;
}

// Square
int square(int x) {
    int result = x * x;
    std::cout << "The square is: " << result << std::endl;
    return result;
}

// Square root
double squareRoot(int x) {
    if (x < 0) {
        std::cout << "Error: Cannot compute square root of a negative number." << std::endl;
        return 0.0;
    }
    double root = std::sqrt(x);
    std::cout << "The square root is: " << root << std::endl;
    return root;
}

int main() {
    int num1, num2;
    
    std::cout << "Enter two numbers: ";
    std::cin >> num1 >> num2;
    
    // Perform calculations
    add(num1, num2);
    subtract(num1, num2);
    multiply(num1, num2);
    divide(num1, num2);
    square(num1);
    squareRoot(num2);
    
    return 0;
}

