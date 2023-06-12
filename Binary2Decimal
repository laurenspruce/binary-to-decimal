import java.util.Scanner;

public class Main {
    public static void main(String[] args) {

        //Creating Scanner
        Scanner in = new Scanner(System.in);

        //User input
        System.out.println("Please enter up to 8 binary digits: ");
        String digits = in.nextLine();

        //Validating the input
        if (!isValidBinary(digits)) {
            System.out.println("Invalid input! Please enter a binary number containing only 0s and 1s.");
            return;
        }

        // Checking the length of the input
        if (digits.length() > 8) {
            System.out.println("Please enter binary containing a maximum of 8 digits!");
        }

        // Converting Binary to Decimal
        int decimal = binaryToDecimal(digits);
        System.out.println("Decimal Equivalent: " + decimal);
    }

    // Function to validate the binary input
    public static boolean isValidBinary(String binary) {
        for (char c : binary.toCharArray()) {
            if (c != '0' && c != '1') {
                return false;
            }
        }
        return true;
    }

    // Function to convert binary to decimal
    public static int binaryToDecimal(String binary) {
        int decimal = 0;
        int power = binary.length() - 1;

        for (char c : binary.toCharArray()) {
            int digit = c - '0'; // Convert char to int

            decimal += digit * Math.pow(2, power);
            power--;
        }
        return decimal;
    }

}
