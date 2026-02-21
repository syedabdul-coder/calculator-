A simple Object-Oriented Programming (OOP) based calculator in Java.
This project demonstrates the use of:

Classes

Objects

Methods

Encapsulation

Switch statements

📌 Features

✔ Uses a separate Calculator class
✔ Performs addition, subtraction, multiplication, division
✔ Handles division by zero
✔ Clean OOP structure
✔ Beginner friendly

💻 Project Structure
BasicCalculatorOOP/
│
├── Calculator.java
└── Main.java

|--------------------------------------|


📄 Main.java
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);
        Calculator calculator = new Calculator();

        System.out.println("===== OOP Java Calculator =====");

        System.out.print("Enter first number: ");
        double num1 = sc.nextDouble();

        System.out.print("Enter operator (+, -, *, /): ");
        char operator = sc.next().charAt(0);

        System.out.print("Enter second number: ");
        double num2 = sc.nextDouble();

        double result = 0;

        switch (operator) {
            case '+':
                result = calculator.add(num1, num2);
                break;

            case '-':
                result = calculator.subtract(num1, num2);
                break;

            case '*':
                result = calculator.multiply(num1, num2);
                break;

            case '/':
                result = calculator.divide(num1, num2);
                break;

            default:
                System.out.println("Invalid operator!");
                sc.close();
                return;
        }

        System.out.println("Result = " + result);
        sc.close();
    }
}
▶ How to Run
java Calculator.java Main.java
java Main
📚 OOP Concepts Used

Class → Calculator

Object → calculator

Methods → add(), subtract(), multiply(), divide()

Encapsulation → Logic separated inside class

🎯 Perfect For

Java beginners

OOP practice

College assignments

GitHub portfolio project
