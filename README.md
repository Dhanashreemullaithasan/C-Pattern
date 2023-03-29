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
public class Exercise33
{
    public static void Main()
    {
        int rows, c = 1, a, i, j;

        Console.Write("rows: ");
        rows = Convert.ToInt32(Console.ReadLine());
        for (i = 0; i < rows; i++)
        {
            for (a = 1; a <= rows - i; a++)
            {
                Console.Write(" ");
            }
            for (j = 0; j <= i; j++)
            {
                if (j == 0 || i == 0)
                {
                    c = 1;
                }
                else
                {
                    c = c * (i - j + 1) / j;
                }
                Console.Write("{0} ", c);
            }
            Console.Write("\n");
        }
    }
}

```
## Output:
![Screenshot 2023-03-21 162800](https://user-images.githubusercontent.com/94165415/228642738-8f906bb1-4d5d-4b26-bca6-6bbeb96a5b48.png)

## Result:
Thus the C# program to print the pascal's triangle is executed successfully.
