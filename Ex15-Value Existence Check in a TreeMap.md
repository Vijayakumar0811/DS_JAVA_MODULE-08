# Ex15 Value Existence Check in a TreeMap

## NAME: VIJAYAKUMAR S
## REG NO: 212224040359
## DATE:28-02-2026
## AIM:
To write a Java program that checks whether a given value exists in a TreeMap.

## Algorithm
1. Start the program.
2. Create an empty TreeMap<Integer, String> named map.
3. Read an integer.
4. Repeat the following steps for i = 0 to n–1.
5. Read a string.
6. Check whether the value exists in the TreeMap by print.
7.  Stop the program.

## Program:

```
import java.util.*;
public class TreeMapValueExistenceCheck {

    public static void checkValue(TreeMap<Integer, String> map, String searchValue) {
        if (map.containsValue(searchValue))
            System.out.println("Value \"" + searchValue + "\" exists in the TreeMap.");
        else
            System.out.println("Value \"" + searchValue + "\" does not exist in the TreeMap.");
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        TreeMap<Integer, String> map = new TreeMap<>();

        int n = sc.nextInt();

        for (int i = 0; i < n; i++) {
            int key = sc.nextInt();
            sc.nextLine();  
            String value = sc.nextLine();
            map.put(key, value);
        }
        String searchValue = sc.nextLine();

        checkValue(map, searchValue);
        sc.close();
    }
}
```

## Output:
<img width="1127" height="744" alt="image" src="https://github.com/user-attachments/assets/1302680a-87fa-4a56-82cb-fc4676f1162d" />

## Result:
Thus, the program successfully checks whether a specified value exists in a TreeMap using the containsValue() method.
