# java-assignment-2
program to prompt students to enter marks for 5 units and calculate the average
import java.util.Scanner;

public class AverageMarks {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.println("Enter the marks for five units:");

        double totalMarks = 0;

        for (int i = 1; i <= 5; i++) {
            System.out.print("Unit " + i + ": ");
            double marks = scanner.nextDouble();
            totalMarks += marks;
        }

        double average = totalMarks / 5;

        System.out.printf("Average marks: %.2f%n", average);

        scanner.close();
    }
}
