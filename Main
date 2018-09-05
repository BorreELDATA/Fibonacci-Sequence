public class Main {

    static long previousNumber = 0;
    static long previousResult = 1;
    static long result = 0;
    static long limit = Long.MAX_VALUE;
    static int fibonacciLimit = 92;
    static final char separator = ',';

    public static void main(String[] args) {
        printFibonacciSequence();
    }

    static void printFibonacciSequence() {
        System.out.println("Fibonacci Sequence");
        for (int i = 1; result < limit && i <= fibonacciLimit; i++) {
            previousNumber = previousResult;
            previousResult = result;
            result = previousNumber + previousResult;
            System.out.println("F" + i + "\t\t" + formatNumber(result));
        }
    }

    static String formatNumber(long number) {
        final StringBuilder builder = new StringBuilder();
        final String numberAsString = String.valueOf(number);
        final char[] characters = numberAsString.toCharArray();
        final int length = characters.length;

        for (int i = 0; i < length; i++) {
            final int j = length - i;
            if (j % 3 == 0 && j != length) builder.append(separator);
            builder.append(characters[i]);
        }
        return builder.toString();
    }
}
