# Java-OOP

/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 */

package com.mycompany.loy.a;

/**
 *
 * @author Student
 */
import java.util.Scanner;

public class LoyA {
    public void add(int number1, int number2) {
        int sum = number1 + number2;
        System.out.println("The sum is: " + sum);
    }
    public void product(int number1, int number2) {
        int product = number1 * number2;
        System.out.println("The product is: " + product);
    }
    public void Subtraction(int number1, int number2) {
        int difference = number1 - number2;
        System.out.println("The difference is: " + difference);
    }
    public void division(int number1, int number2) {
        int quotient = number1 / number2;
        System.out.println("The quotient is: " + quotient);
    }
    public void average(int number1, int number2) {
        int average = (number1 + number2) / 2;
        System.out.println("The average is: " + average);
    }
    public void option(){
        System.out.println("Input operation: \n 1: Addition \n 2: subtraction \n 3: Multiplication \n 4: Division \n 5: Average");
        int add = 1;
        int Subtraction = 2;
        int Multiplication = 3;
        int Division = 4;
        int average = 5;
        try(Scanner a = new Scanner(System.in) ){
            System.out.println("Input Operation: ");
            int option = a.nextInt();
            if(option == add){
                LoyA lmadd = new LoyA();
                System.out.println("Enter first number: ");
                int number1 = a.nextInt();
                System.out.println("Enter second number: ");
                int number2 = a.nextInt();
                lmadd.add(number1, number2);
            }
            else if(option == Subtraction){
                LoyA lmSubtraction = new LoyA();
                System.out.println("Enter first number: ");
                int number1 = a.nextInt();
                System.out.println("Enter second number: ");
                int number2 = a.nextInt();
                lmSubtraction.Subtraction(number1, number2);
            }
            else if(option == Multiplication){
                LoyA lmMultiplication = new LoyA();
                System.out.println("Enter first number: ");
                int number1 = a.nextInt();
                System.out.println("Enter second number: ");
                int number2 = a.nextInt();
                lmMultiplication.product(number1, number2);
            }
            else if(option == Division){
                LoyA lmDivision = new LoyA();
                System.out.println("Enter first number: ");
                int number1 = a.nextInt();
                System.out.println("Enter second number: ");
                int number2 = a.nextInt();
                lmDivision.division(number1, number2);
            }
            else if(option == average){
                LoyA lmaverage = new LoyA();
                System.out.println("Enter first number: ");
                int number1 = a.nextInt();
                System.out.println("Enter second number: ");
                int number2 = a.nextInt();
                lmaverage.average(number1, number2);
            }
            else{
                System.out.println("Invalid Input!");
            }
        }
        catch(Exception e){
            System.out.println("Invalid Input");
        }
    }
    public static void main(String[] args) {
        LoyA calculator = new LoyA();
        calculator.option();
    }
}
