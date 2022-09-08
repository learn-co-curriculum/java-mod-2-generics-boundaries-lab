# Generics Boundaries Lab

## Learning Goals

- Create a generic static method with an upper bound

## Instructions

Create a method that returns the average of a list of numbers. Make sure the
method is restricted to dealing with numbers and that your code will not
compile if you try to pass in a list of objects that are not actually numbers.

## Starter Code and Hints

Consider the following starter code to help you get started and test your code:

```java
import java.util.List;

public class GenericsPractice {
    // implement the public averageList method here
    
    public static void main(String[] args) {
        List<Integer> intList = List.of(1, 2, 3, 4, 5);
        System.out.println(averageList(intList)); // 3.0

        List<Double> doubleList = List.of(1.0, 2.0, 3.0, 4.0, 5.0);
        System.out.println(averageList(doubleList)); // 3.0       
    }
}
```

Hints:

- You need to use an upper bound wildcard.
- You can use the `Double` class as the precision for your calculation.
- The average is the sum divided by the number of elements in the list.

## Sample Output

If you run the code above with what is in the `main()` method, you should see
an output like this:

```plaintext
3.0
3.0
```
