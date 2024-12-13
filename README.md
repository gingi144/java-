import java.util.Scanner;

public class Shapes {

    private double width;
    private double height;

    // First method: Get dimensions from the user
    public void getDimensions() {
        Scanner scanner = new Scanner(System.in);

        System.out.print("Enter the width of the rectangle: ");
        width = scanner.nextDouble();

        System.out.print("Enter the height of the rectangle: ");
        height = scanner.nextDouble();
    }

    // Second method: Compute area
    public double computeArea(double width, double height) {
        return width * height;
    }

    // Third method: Display area
    public void displayArea(double area) {
        System.out.println("The area of the rectangle is: " + area);
    }

    // Main method
    public static void main(String[] args) {
        Shapes rectangle = new Shapes();

        // Get dimensions
        rectangle.getDimensions();

        // Compute area
        double area = rectangle.computeArea(rectangle.width, rectangle.height);

        // Display area
        rectangle.displayArea(area);
    }
}
