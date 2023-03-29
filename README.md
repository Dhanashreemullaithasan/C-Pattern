# Pattern

## Aim:

To write a C# program for a pascal's triangle.

## Equipment Required:

Visual Studio.

## Algorithm:
Step 1: Start the program.

Step 2: Create a class and declare two variables rows,Val using integer datatype.

Step 3: Using nested for loop create a pascal's triangle.

Step 4: Stop the execution.

## Program:
```
using System;
namespace Pattern
{
    public class pascal
    {
        public static void Main(string[] args)
        {
            Console.WriteLine("Pascal`s Triangle : ");
            int rows = 5, num = 1;
            for(int i=0;i<rows;i++)
            {
                for(int k=1;k<rows-i;k++)
                {
                    Console.Write(" ");
                }
                for(int j=0;j<=i;j++)
                {
                    if(i==0 || j==0)
                    {
                        num = 1;
                    }
                    else
                    {
                        num = num * (i - j + 1) / j;
                    }
                    Console.Write(num + " ");
                }
                Console.WriteLine();
            }
        }
    }
 }
```
## Output:
![Screenshot 2023-03-21 162800](https://user-images.githubusercontent.com/94165415/228642738-8f906bb1-4d5d-4b26-bca6-6bbeb96a5b48.png)

## Result:
Thus the C# program to print the pascal's triangle is executed successfully.
