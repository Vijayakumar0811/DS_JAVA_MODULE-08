# Ex14 Tracking the First Unique Number in a Stream using LinkedHashMap

## NAME: VIJAYAKUMAR S
## REG NO: 212224040359
## DATE: 28-02-20226
## AIM:
To implement a program that tracks the first unique (non-repeating) number in a stream of integers using a LinkedHashMap.

## Algorithm
1. Start the program.
2. Read an integer n (the number of inputs in the stream).
3. Create an empty LinkedHashMap<Integer, Integer> named map.
4. Repeat the following steps for each of the n numbers.
5. After processing all numbers, end the program.
  

## Program:
```

import java.util.*;

public class FirstUniqueNumberStream {

    public static void processStream(int n, Scanner sc) {
        LinkedHashMap<Integer, Integer> map = new LinkedHashMap<>();
        for (int i = 0; i < n; i++) {
            int num = sc.nextInt();
            map.put(num, map.getOrDefault(num, 0) + 1);
            boolean found = false;
            for (Map.Entry<Integer, Integer> entry : map.entrySet()) {
                if (entry.getValue() == 1) {
                    System.out.println("First unique number: " + entry.getKey());
                    found = true;
                    break;
                }
            }
            if (!found) {
                System.out.println("No unique number");
            }
        }
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        processStream(n, sc);
        sc.close();
    }
}

```

## Output:

<img width="942" height="659" alt="image" src="https://github.com/user-attachments/assets/150c79ce-1c29-4d7f-8aa3-1f912a75f536" />

## Result:
The program successfully tracks and returns the first unique number at any point in the integer stream using a LinkedHashMap.
