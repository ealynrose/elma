int[] numbers; // Declaration of an integer array
 int[] numbers = new int[5]; // An array of 5 integers initialized to default values (0)
 int[] numbers = { 1, 2, 3, 4, 5 }; // An array initialized with specific values
 int firstNumber = numbers[0]; // Accessing the first element
numbers[1] = 10; // Changing the second element to 10
4. Iterating Through Arrays
for (int i = 0; i < numbers.Length; i++)
{
    Console.WriteLine("Element " + i + ": " + numbers[i]);
}
foreach (int number in numbers)
{
    Console.WriteLine("Number: " + number);
}
int[,] matrix = new int[3, 3]; // A 3x3 matrix

// Initializing elements
matrix[0, 0] = 1;
matrix[0, 1] = 2;
matrix[0, 2] = 3;
// And so on...
for (int i = 0; i < matrix.GetLength(0); i++)
{
    for (int j = 0; j < matrix.GetLength(1); j++)
    {
        Console.Write(matrix[i, j] + " ");
    }
    Console.WriteLine();
}
static void PrintArray(int[] arr)
{
    foreach (var item in arr)
    {
        Console.WriteLine(item);
    }
}

// Usage:
PrintArray(numbers);
