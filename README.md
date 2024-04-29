# si
-----------------java--------------------
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        double principal = scanner.nextDouble();
        double rate = scanner.nextDouble() / 100; // convert percentage to decimal
        int years = scanner.nextInt();
        double interest = principal * rate * years;
        double totalAmount = principal + interest;
        System.out.printf("%.2f\n%.2f\n", interest, totalAmount);
        double discount = interest * 0.02; // 2% discount on total interest
        double amountBack = discount;
        totalAmount -= discount;
        System.out.printf("%.2f\n%.2f", amountBack, totalAmount);
        scanner.close();
    }
}

   
