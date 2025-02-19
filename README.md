# operation-using-package-program-
package math_operations;
public class Calculator {
public int add(int a, int b) {
return a + b;
}
public int subtract(int a, int b) {
return a - b;
}
public int multiply(int a, int b) {
return a * b;
}
public double divide(int a, int b) {
if (b != 0) {
return (double) a / b;
} else {
System.out.println(&quot;Cannot divide by zero!&quot;);
return Double.NaN; 
}
}
}

package math_operations;
public class MathUtils {
public double calculateSquareRoot(double num) {
if (num &gt;= 0) {
return Math.sqrt(num);
} else {
System.out.println(&quot;Cannot calculate square root of a negative number!&quot;);
return Double.NaN;

}
}
}

public class MathOperationsApp {
public static void main(String[] args) {

math_operations.Calculator calculator = new math_operations.Calculator();
math_operations.MathUtils mathUtils = new math_operations.MathUtils();

System.out.println(&quot;Addition: &quot; + calculator.add(5, 3));
System.out.println(&quot;Subtraction: &quot; + calculator.subtract(8, 4));
System.out.println(&quot;Multiplication: &quot; + calculator.multiply(2, 6));
System.out.println(&quot;Division: &quot; + calculator.divide(10, 2));

System.out.println(&quot;Square Root: &quot; + mathUtils.calculateSquareRoot(25));
System.out.println(&quot;Square Root of -9: &quot; + mathUtils.calculateSquareRoot(-9));
}
}
Output:
Addition: 8
Subtraction: 4
Multiplication: 12
Division: 5.0
Square Root: 5.0
Cannot calculate square root of a negative number!
Square Root of -9: NaN
