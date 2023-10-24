# Find-the-Factorial-of-the-Number-using-Recursion-in-Java

Factorial of a Number using Recursion in Java
Here, in this page we will discuss the program to find the factorial of a number using recursion in Java programming Language. We will discuss various methods to solve the given problem.

Factorial of a Number using Recursion in Java
Method Discussed :
Method 1 : Using Recursion
Method 2 : Using Iteration.
Let’s discuss them one by one in brief,

Method 1:
Call function getFactorial(num)
Set base case when num== 0 return 1
Other cases return num * getFactorial(num-1);
Time and Space Complexity :
Time complexity: O(N)
Space complexity: O(1)
Auxiliary Space complexity (Function call stack): O(N)
Factorial of Number using Recursion in java
Run
class Main {
    // method to find factorial of given number
    static int factorial(int n)
    {
        if (n == 0)
            return 1;
 
        return n * factorial(n - 1);
    }
 
    // Driver method
    public static void main(String[] args)
    {
        int num = 5;
        System.out.println("Factorial of " + num  + " is " + factorial(5));
    }
}
Output :
Factorial of 5 is 120
Method 2:
Initialize fact = 1
If num < 0 : Print Error as we can’t calculate factorial of a negative number
Else run a iterative loop in iteration of (i) between [1, num]
Set fact = fact * i
Print the value of fact.
Time and Space Complexity :
Time complexity: O(N)
Space complexity: O(1)
Method 2 : Code in Java
Run
class Main {
 
    // Method to find factorial of the given number
    static int factorial(int n)
    {
        int res = 1, i;
        for (i = 2; i <= n; i++)
            res *= i;
        return res;
    }
 
    // Driver method
    public static void main(String[] args)
    {
        int num = 5;
        System.out.println("Factorial of " + num + " is " + factorial(5));
    }
}   
Output :
Factorial of 5 is 120
