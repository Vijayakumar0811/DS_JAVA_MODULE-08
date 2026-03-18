# Ex13 Fill the First 10 Elements of an Array with a Constant using Arrays.fill()

## NAME: VIJAYAKUMAR S
## REG NO: 212224040359
## DATE: 25-02-2026
## AIM:
To write a Java program that fills the first 10 elements of an array with a constant value using the Arrays.fill() method.
## Algorithm
1. Start the program.
2. Read an integer value from the user.
3. Call the function fillArray(10, value).
4. Create an integer array arr of length size.
5. Fill every element of arr with value using Arrays.fill(arr, value).
6. Return the filled array.
7. Store the returned array in arr.
8. Print the message "Array elements:".
9. For each element in arr, print the element.
10. End the program.

## Program:
```
import java.util.*;

public class FillArrayUsingArraysFill {

    public static int[] fillArray(int size, int value) {
        // Type Your Code Here.
        int[] arr = new int[size];
         Arrays.fill(arr,value);
         return arr;
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int value = sc.nextInt();
        int[] arr = fillArray(10, value);
        System.out.println("Array elements:");
        for (int num : arr) {
            System.out.print(num + " ");
        }
        sc.close();
    }
}

```

## Output:
<img width="979" height="326" alt="image" src="https://github.com/user-attachments/assets/f24868be-5b48-439e-85a0-2246b6900bfb" />



## Result:
The program successfully fills the first 10 elements of the array with the constant value 5 using the Arrays.fill() method.
