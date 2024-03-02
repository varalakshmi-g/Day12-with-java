# Day12-with-java

Today I learned and written the code for printing pairs in an array, Here we go...

import java.util.Arrays;

public class PrintAllPairs {
    public static void printPairs(int[] arr) {
        int n = arr.length;
        for (int i = 0; i < n; i++) {
            for (int j = 0; j < n; j++) {
                System.out.println("(" + arr[i] + ", " + arr[j] + ")");
            }
        }
    }

    public static void main(String[] args) {
        int[] arr = {1, 2, 3, 4};
        printPairs(arr);
    }
}

Here is the detailed description of getting output. 

Let's go...

1. Array "arr" is declared and initialized with values {1, 2, 3, 4,}

2. printPairs method wtakes an integer array arr as its parameter, inside this method, length of the array "arr" will be stored in the variable 'n'.

3. Outer loop which is controlled by variable i will iterates over each element of the array from index 0 to n-1.

4. Inner loop which is controlled by variable j will iterates over each element of the array from index 0 to n-1.

5. For each combination of i and j, println statement is executed, which prints a pair of elements from the array.

6. Inside the println statement, the values of arr[i] and arr[j] are concatenated with parentheses and comma to form a pair, which is then printed to the console.

7. In main method printPairs method is called with the arr as an argument, this triggers the execution of printpairs method.

8. As a result of nested loops in the printPairs method, every combination of elements from the arr is printed as a pair. Since there are 4 elements in the array, and the loops iterate over all combinations, the total number of pairs printed is 16 .

output : 
(1, 1)
(1, 2)
(1, 3)
(1, 4)
(2, 1)
(2, 2)
(2, 3)
(2, 4)
(3, 1)
(3, 2)
(3, 3)
(3, 4)
(4, 1)
(4, 2)
(4, 3)
(4, 4)
