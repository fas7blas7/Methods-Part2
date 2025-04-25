1️⃣ VowelsCount 🔤  
Namespace: _1_VowelsCount  
📌 Description:  
Reads a string and counts the number of vowels (both uppercase and lowercase) it contains.

📝 Code:
```csharp
namespace _1_VowelsCount
{
    internal class Program
    {
        static void Main(string[] args)
        {
            string inputText = Console.ReadLine();
            int result = GetVowelsCount(inputText);

            string inputText2 = Console.ReadLine();
            result = GetVowelsCount(inputText);
            Console.WriteLine(result);
        }

        static int GetVowelsCount(string text)
        {
            int result = 0;
            foreach (char letter in text)
            {
                if (letter == 'a'
                    || letter == 'o'
                    || letter == 'u'
                    || letter == 'e'
                    || letter == 'i'
                    || letter == 'A'
                    || letter == 'O'
                    || letter == 'U'
                    || letter == 'E'
                    || letter == 'I'
                    )
                {
                    result++;
                }
            }

            return result;
        }
    }
}
```

2️⃣ Factoreal ➗  
Namespace: _2_Factoreal  
📌 Description:  
Reads two integers, calculates their factorials, and outputs the result of the first divided by the second.

📝 Code:
```csharp
namespace _2_Factoreal
{
    internal class Program
    {
        static void Main(string[] args)
        {
            int firstNumber = int.Parse(Console.ReadLine());
            int secondNumber = int.Parse(Console.ReadLine());

            int firstNumberFactorial = Factorial(firstNumber);
            int secondNumberFactorial = Factorial(secondNumber);

            int result = firstNumberFactorial / secondNumberFactorial;
            Console.WriteLine(result);
        }

        static int Factorial(int n) // n = 5
        {
            int result = 1;
            if (n == 0 || n == 1)
            {
                return result;
            }

            for (int i = n; i >= 2; i--)
            {
                result *= i;
            }

            return result;
        }
    }
}
```
3️⃣ MultiplicationSign ➕➖  
Namespace: _3_Multiplication_Sign  
📌 Description:  
Reads three integers and determines if their product is positive, negative, or zero without actually multiplying.

📝 Code:
```csharp
namespace _3_Multiplication_Sign
{
    internal class Program
    {
        static void Main(string[] args)
        {
            int a = int.Parse(Console.ReadLine());
            int b = int.Parse(Console.ReadLine());
            int c = int.Parse(Console.ReadLine());

            string result = GetMultiplicationSign(a, b, c);
            Console.WriteLine(result);
        }

        static string GetMultiplicationSign(int a, int b, int c)
        {
            string result = "";
            if (IsAnyNumberZero(a, b, c))
            {
                result = "zero";
            }
            else if (GetNegativeNumbersCount(a, b, c) % 2 == 0)
            {
                result = "positive";
            }
            else
            {
                result = "negative";
            }

            return result;
        }

        static int GetNegativeNumbersCount(int a, int b, int c)
        {
            int negativeNumbers = 0;
            if (a < 0)
            {
                negativeNumbers++;
            }

            if (b < 0)
            {
                negativeNumbers++;
            }

            if (c < 0)
            {
                negativeNumbers++;
            }

            return negativeNumbers;
        }

        static bool IsAnyNumberZero(int a, int b, int c)
        {
            if (a == 0 || b == 0 || c == 0)
            {
                return true;
            }

            return false;
        }
    }
}

📅 Updated Commit Progress:

📅 Current Progress: 396 commits  
📊 Progress Bar:  
██████████████████████████████░ 79.2% (396/500)

📌 Milestones:  
✅ 100 commits  
✅ 200 commits  
✅ 300 commits  
🔲 400 commits  
🔲 500 commits (🎉)  
🎯 Commit Progress Tracker  

🚀 Goal: 500 commits in 2025  
📅 Current Progress: 396 commits  
🚀 Goal: 500 commits in 2025
📅 Current Progress: 394 commits
