# Coding Question Exercise

Poll: pollEv.com/nicmatt

## Question 1 - Random Star
Write a method named randomStar that takes two parameters, a Random object `rand` and an integer `max`.

Your method should generate a random number between 5 and 19 (inclusive on both ends), and print the * (asterisk) character as much as the random number that you generate in a single line.

Your method will keep generating a new random number between 5 and 19 (inclusive on both ends) and printing out the * characters until the random number generated is bigger than or equal to `max`.

For example, the method call `randomStar(rand, 14)` will print:

```
***********
*****
*******
*******
********
**********
*********
************
**********
***********
***********
**************
```

The list of Random number generated above:

```
11
5
7
7
8
10
9
12
10
11
11
14
```

> The list of random number below is meant to help you understand the code. It IS NOT part of the program's output!

Notice how the program stops after 14 *'s have been printed since 14 (the random number generated prior to printing the last line in the example above) is greater than or equal to the parameter num, 14.

You should not change any code in the main method!

---
### **Caution!!!**
It's important that your method utilizes all the random number that you generate. In particular, make sure that you are utilizing the first and the last random number that you generate to print the * characters.

---

### **Starter Code**

```java
import java.util.*;
public class RandomStar {
    public static void main(String[] args) {
        // Note: 2063064142 is called a random seed.
        // You can ignore this value!
        Random rand = new Random(2063064142);
        randomStar(rand, 12);

        System.out.println();
        randomStar(rand, 19);
    }

}
```

> There are two method calls in the main method. Feel free to comment one of the method call when you are testing your code!
---