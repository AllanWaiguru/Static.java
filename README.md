# Static.java
import java.util.Scanner;

public class TriangleAreaCalculator {
    public TriangleAreaCalculator() {
        // Constructor
    }

    public void enterBaseAndHeight() {
        Scanner input = new Scanner(System.in);
        System.out.print("Enter the base of the triangle: ");
        double base = input.nextDouble();
        System.out.print("Enter the height of the triangle: ");
        double height = input.nextDouble();
        calculateArea(base, height);
    }

    public static void calculateArea(double base, double height) {
        double area = (base * height) / 2;
        displayArea(area);
    }

    public static void displayArea(double area) {
        System.out.println("The area of the triangle is: " + area);
    }

    public static void main(String[] args) {
        TriangleAreaCalculator calculator = new TriangleAreaCalculator();
        calculator.enterBaseAndHeight();
    }
}
