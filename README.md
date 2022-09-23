# Ex05-Rec-JaggedArray
## Aim:
To write a C# program to create a sample CPU usage on a network with 4 nodes using a jagged array.
## Algorithm:
### Step1:


## Program:
~~~
using System;
namespace abhi
{
    public class Program
    {
        public static void Main(string[] args)
        {
            int[][] array = new int[4][];
            array[0] = new int[4];
            array[1] = new int[3];
            array[2] = new int[2];
            array[3] = new int[5];
            for(int i = 0; i < 4; i++)
            {
                for(int j= 0; j < array[i].Length; j++)
                {
                    array[i][j] = i*j+70;
                }
            }
            for (int i = 0; i < 4; i++)
            {
                for (int j = 0; j < array[i].Length; j++)
                {
                    Console.WriteLine("Usage of CPU in node "+i+" is " + array[i][j]+"%");
                }
                Console.WriteLine();
            }
        }
    }
}
~~~

## Output:
![image](https://user-images.githubusercontent.com/66360846/191891798-5a409741-f99e-4575-b241-6820401c4c8f.png)


## Result:
A sample CPU usage on a network with 4 nodes using a jagged array is executed successfully.
