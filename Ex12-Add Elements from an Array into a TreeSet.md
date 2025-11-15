# Ex12 Add Elements from an Array into a TreeSet
## DATE:
## AIM:
To write a Java program that adds elements from an array into a TreeSet and displays the elements in sorted order.
## Algorithm
1. 
2. 
3. 
4.  
5.   

## Program:
```java
/*
Program that adds elements from an array into a TreeSet and displays the elements in sorted order.
Developed by: ASWIN B
Register Number: 212224110007  
*/

import java.util.*;

public class ArrayToTreeSet {

    public static TreeSet<Integer> convertArrayToTreeSet(int[] arr) {
        List<Integer> list = new ArrayList<>();
        for(int x : arr){
            list.add(x);
        }
        
        TreeSet<Integer> treeSet = new TreeSet<>(list);
        return treeSet;
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int[] arr = new int[n];
        for (int i = 0; i < n; i++) {
            arr[i] = sc.nextInt();
        }

        TreeSet<Integer> treeSet = convertArrayToTreeSet(arr);
        System.out.println("Elements in TreeSet:");
        for (int num : treeSet) {
            System.out.println(num);
        }

        sc.close();
    }
}

```

## Output:
<img width="624" height="436" alt="image" src="https://github.com/user-attachments/assets/869f72c0-2cfe-4e38-a11e-669968f0a796" />



## Result:
The program successfully adds elements from an array into a TreeSet.
