
import java.util.Scanner;

class caculater {
    caculater() {
    }

    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
        System.out.println("Choose an operator: +, -, *, or /");
        char operator = input.next().charAt(0);
        System.out.println("Enter first number");
        Double number1 = input.nextDouble();
        System.out.println("Enter second number");
        Double number2 = input.nextDouble();
        switch (operator) {
            case '*':
                Double result = number1 * number2;
                System.out.println(number1 + " * " + number2 + " = " + result);
                break;
            case '+':
                Double result = number1 + number2;
                System.out.println(number1 + " + " + number2 + " = " + result);
                break;
            case ',':
            case '.':
            default:
                System.out.println("Invalid operator!");
                break;
            case '-':
                Double result = number1 - number2;
                System.out.println(number1 + " - " + number2 + " = " + result);
                break;
            case '/':
                Double result = number1 / number2;
                System.out.println(number1 + " / " + number2 + " = " + result);
        }

        input.close();
    }
}
