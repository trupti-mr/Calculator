#include <iostream>
#include <cmath>

// Addition
double add(double x, double y) {
    double sum = x + y;
    std::cout << "The sum is: " << sum << std::endl;
    return sum;
}

// Subtraction
double subtract(double x, double y) {
    double difference = x - y;
    std::cout << "The difference is: " << difference << std::endl;
    return difference;
}

// Multiplication
double multiply(double x, double y) {
    double product = x * y;
    std::cout << "The product is: " << product << std::endl;
    return product;
}

// Division
double divide(double x, double y) {
    if (y == 0) {
        std::cout << "Error: Division by zero is not allowed." << std::endl;
        return 0.0;
    }
    double quotient = x / y;
    std::cout << "The quotient is: " << quotient << std::endl;
    return quotient;
}

// Square
double square(double x) {
    double result = x * x;
    std::cout << "The square is: " << result << std::endl;
    return result;
}

// Square root
double squareRoot(double x) {
    if (x < 0) {
        std::cout << "Error: Cannot compute square root of a negative number." << std::endl;
        return 0.0;
    }
    double root = std::sqrt(x);
    std::cout << "The square root is: " << root << std::endl;
    return root;
}

// Exponentiation
double power(double x, double y) {
    double result = std::pow(x, y);
    std::cout << x << " raised to the power of " << y << " is: " << result << std::endl;
    return result;
}

// Logarithm
double logarithm(double x) {
    if (x <= 0) {
        std::cout << "Error: Invalid input for logarithm." << std::endl;
        return 0.0;
    }
    double result = std::log10(x);
    std::cout << "The logarithm (base 10) of " << x << " is: " << result << std::endl;
    return result;
}

int main() {
    double num1, num2;
    
    std::cout << "Enter two numbers: ";
    std::cin >> num1 >> num2;
    
    // Perform calculations
    add(num1, num2);
    subtract(num1, num2);
    multiply(num1, num2);
    divide(num1, num2);
    square(num1);
    squareRoot(num2);
    
    // Additional scientific functions
    power(num1, num2);
    logarithm(num2);
    
    return 0;
}
