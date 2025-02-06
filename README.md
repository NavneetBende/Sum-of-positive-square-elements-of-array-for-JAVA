Sum of positive square elements of the array
Here we will learn about Sum of positive square elements of array.

For this program, we need to find the square of every element and add all these square elements.

Example
Input:       1 2 3 4 5

Square:     1 4 9 16 25

sum:        1+4+9+16+25=55

now we will see the working of program and java program of the square sum of elements.

Square sum
Working
Step 1. Initialize arrays.

Step 2. Declare the scanner class for taking input.

Step 3. take array size from the user.

Step 4. Take an element of the array from the user.

Step 5.  Print the return value of the function SquareSum.

SquareSum(int a[], int size)

Step 1. Initialise two-variable sum and square with zero.

Step 2.  Declare loop from zero to size.

Step 3.  Inside the loop calculate the square of every element.

Step 4.  Inside the loop calculate the sum, add the sum with a square.

Step 5. Return sum.

C	JAVA	Python
import java.util.Scanner;
public class Main
{
    public static int SquareSum(int a[],int size) 
    {
        int sum=0;
        int square=0;
        //for loop to square and sum of elements
        for(int i=0;i<size;i++)
        {
            square=a[i]*a[i];
            sum=sum+square;
        }
        //return the sum variable;
        return sum;
    }

    public static void main(String[] args) 
    {
        int j=0;
        //create array 
        int[] arr=new int[40];
        //declare the scanner class
        Scanner sc=new Scanner(System.in);
        //take size of an array
        System.out.println("enter size");
        int size=sc.nextInt();
         //take array element
        System.out.println("enter element");
        for(int i=0;i<size;i++)
              arr[i]=sc.nextInt();
        //print sum from calling the fuction SquareSum
        System.out.print("square sum of element "+SquareSum(arr,size));
     }
}
Output
enter size 
4
enter element
1
2
3
4
square sum of element 30
