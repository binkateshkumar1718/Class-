// 1st program
// public class Main {
//     public static void main(String[] args){
//         System.out.println("Name : Shubh Shrivastava");
//     }
// }

// //2nd program
// public class Main {
//     public static void main(String[] args){
//         System.out.println("Address : Jhansi, U.P.");
//     }
// }

//3rd program
// import java.util.* ;
// public class Main {
//     public static void main(String[] args){
//         Scanner sc = new Scanner (System.in);
//         System.out.println("Enter the value of a: ");
//         int a=sc.nextInt();
//         System.out.println("Enter the value of b: ");
//         int b=sc.nextInt();
//         System.out.println("The Addition of a and b is "+(a+b));
//         System.out.println("The Subtraction of a and b is "+(a-b));
//         System.out.println("The Multiplication of a and b is "+(a*b));
//         System.out.println("The Division of a and b is "+(a/b));
        
//     }
// }

//4th program
// public class DataTypesInfo {
//     public static void main(String[] args) {
//         // Primitive Data Types
//         System.out.println("---- Primitive Data Types ----");

//         System.out.println("byte:");
//         System.out.println("Size: " + Byte.BYTES + " bytes");
//         System.out.println("Range: " + Byte.MIN_VALUE + " to " + Byte.MAX_VALUE);

//         System.out.println("\nshort:");
//         System.out.println("Size: " + Short.BYTES + " bytes");
//         System.out.println("Range: " + Short.MIN_VALUE + " to " + Short.MAX_VALUE);

//         System.out.println("\nint:");
//         System.out.println("Size: " + Integer.BYTES + " bytes");
//         System.out.println("Range: " + Integer.MIN_VALUE + " to " + Integer.MAX_VALUE);

//         System.out.println("\nlong:");
//         System.out.println("Size: " + Long.BYTES + " bytes");
//         System.out.println("Range: " + Long.MIN_VALUE + " to " + Long.MAX_VALUE);

//         System.out.println("\nfloat:");
//         System.out.println("Size: " + Float.BYTES + " bytes");
//         System.out.println("Range: " + Float.MIN_VALUE + " to " + Float.MAX_VALUE);

//         System.out.println("\ndouble:");
//         System.out.println("Size: " + Double.BYTES + " bytes");
//         System.out.println("Range: " + Double.MIN_VALUE + " to " + Double.MAX_VALUE);

//         System.out.println("\nchar:");
//         System.out.println("Size: " + Character.BYTES + " bytes");
//         System.out.println("Range: " + (int) Character.MIN_VALUE + " to " + (int) Character.MAX_VALUE);

//         System.out.println("\nboolean:");
//         System.out.println("Size: JVM dependent (usually 1 bit to 1 byte)");
//         System.out.println("Range: " + Boolean.FALSE + " to " + Boolean.TRUE);

//         // Non-Primitive  Data Types
//         System.out.println("\n---- Non-Primitive (Reference) Data Types ----");
//         System.out.println("Examples: String, Array, Class, Interface, etc.");
//         System.out.println("Size depends on the object and JVM implementation.");
//         System.out.println("No fixed range like primitives.");
//     }
// }

//5th program

// import java.util.Scanner;

// public class MeterToFeetConverter {
//     public static void main(String[] args) {
//         Scanner sc = new Scanner(System.in);

//         // Input in meters
//         System.out.print("Enter length in meters: ");
//         double meters = sc.nextDouble();

//         // Conversion: 1 meter = 3.28084 feet
//         double feet = meters * 3.28084;

//         // Output result
//         System.out.println(meters + " meters is equal to " + feet + " feet.");

//         sc.close();
//     }
// }

//program 6
import java.util.Scanner;

public class QuadraticEquationSolver {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        // Reading input
        System.out.print("Enter coefficient a: ");
        double a = scanner.nextDouble();
        System.out.print("Enter coefficient b: ");
        double b = scanner.nextDouble();
        System.out.print("Enter coefficient c: ");
        double c = scanner.nextDouble();

        // Calculate discriminant
        double discriminant = b * b - 4 * a * c;

        System.out.println("\nQuadratic Equation: " + a + "x² + " + b + "x + " + c + " = 0");

        // Checking nature of roots
        if (discriminant > 0) {
            double root1 = (-b + Math.sqrt(discriminant)) / (2 * a);
            double root2 = (-b - Math.sqrt(discriminant)) / (2 * a);
            System.out.println("Two real solutions:");
            System.out.println("Root 1 = " + root1);
            System.out.println("Root 2 = " + root2);
        } else if (discriminant == 0) {
            double root = -b / (2 * a);
            System.out.println("One real solution:");
            System.out.println("Root = " + root);
        } else {
            System.out.println("No real solutions. Discriminant is negative.");
        }

        scanner.close();
    }
}
