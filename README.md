# HW3

namespace HW3_1
{
    class Program
    {
        static void Main(string[] args)
        {
            int[,] matrix = new int[5,5];
            matrix[1,3] = 1;
            matrix[3,1] = 1;
            matrix[0, 4] = 1;
            matrix[4, 0] = 1;
            matrix[2, 2] = 1;
            for (int i = 0; i < matrix.GetLength(0); i++)
            {
                for(int j = 0; j < matrix.GetLength(1); j++)
                {
                    Console.Write($"{matrix[i,j]} ");
                }
                Console.WriteLine();
            }
            Console.ReadLine();
        }
    }
}

namespace HW3_2
{
    class Program
    {
        static void Main(string[] args)
        {
            string[,] myArray = new string[,]
            {
                {"Semenev","Semakov","Nevikov","Sorikov","Shumachin"},
                {"336-43-32","336-43-33","336-43-34","336-43-35","336-43-36"},
                {"sem@ekb.ru","sma@ekb.ru","nev@ekb.ru","sor@ekb.ru","shu@ekb.ru" }
            };
            int height = myArray.GetLength(0);//вводим переменную для получения длины массива по вертикали
            int width = myArray.GetLength(1);//вводим переменную для получения длины массива по горизонтали

            for (int i = 0; i < height; i++) // внешний цикл с выводом данных по вертикали

            {
                for (int j = 0; j < width; j++) //вложенный цикл с выводом данных по горизонтали
                {
                    Console.Write(myArray[i, j] + " \t "); //для вывода массива как в условии задачи используем Write вместо WriteLine
                }
                Console.WriteLine();// вводим для разделения между столбцами

                Console.ReadLine();
            }
        }
    }
}

namespace HW3_3
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("введите строку");
            string randomWord = Console.ReadLine();
            char[] array = randomWord.ToCharArray();
            Array.Reverse(array);
            Console.WriteLine(array);

            Console.ReadLine();
        }
    }
}

namespace HW3_4
{
    class Program
    {
        static void Main(string[] args)
        {
            char[,] matrix = new char [10, 10];
            matrix[0, 0] = 'O'; matrix[0, 1] = 'X'; matrix[0, 2] = 'O'; matrix[0, 3] = 'O'; matrix[0, 4] = 'X'; matrix[0, 5] = 'X'; matrix[0, 6] = 'O';
            matrix[0, 7] = 'X'; matrix[0, 8] = 'X'; matrix[0, 9] = 'X';
            matrix[1, 0] = 'X'; matrix[1, 1] = 'X'; matrix[1, 2] = 'X'; matrix[1, 3] = 'X'; matrix[1, 4] = 'X'; matrix[1, 5] = 'X'; matrix[1, 6] = 'X';
            matrix[1, 7] = 'X'; matrix[1, 8] = 'O'; matrix[1, 9] = 'O';
            matrix[2, 0] = 'O'; matrix[2, 1] = 'O'; matrix[2, 2] = 'X'; matrix[2, 3] = 'X'; matrix[2, 4] = 'X'; matrix[2, 5] = 'X'; matrix[2, 6] = 'O';
            matrix[2, 0] = 'O'; matrix[2, 1] = 'O'; matrix[2, 2] = 'X'; matrix[2, 3] = 'X'; matrix[2, 4] = 'X'; matrix[2, 5] = 'X'; matrix[2, 6] = 'O';
            matrix[2, 7] = 'X'; matrix[2, 8] = 'X'; matrix[2, 9] = 'X';
            matrix[3, 0] = 'X'; matrix[3, 1] = 'X'; matrix[3, 2] = 'X'; matrix[3, 3] = 'O'; matrix[3, 4] = 'X'; matrix[3, 5] = 'X'; matrix[3, 6] = 'O';
            matrix[3, 7] = 'X'; matrix[3, 8] = 'X'; matrix[3, 9] = 'X';
            matrix[4, 0] = 'X'; matrix[4, 1] = 'X'; matrix[4, 2] = 'X'; matrix[4, 3] = 'O'; matrix[4, 4] = 'X'; matrix[4, 5] = 'X'; matrix[4, 6] = 'O';
            matrix[4, 7] = 'X'; matrix[4, 8] = 'X'; matrix[4, 9] = 'X';
            matrix[5, 0] = 'X'; matrix[5, 1] = 'X'; matrix[5, 2] = 'X'; matrix[5, 3] = 'O'; matrix[5, 4] = 'X'; matrix[5, 5] = 'X'; matrix[5, 6] = 'O';
            matrix[5, 7] = 'X'; matrix[5, 8] = 'X'; matrix[5, 9] = 'X';
            matrix[6, 0] = 'X'; matrix[6, 1] = 'X'; matrix[6, 2] = 'X'; matrix[6, 3] = 'X'; matrix[6, 4] = 'X'; matrix[6, 5] = 'X'; matrix[6, 6] = 'X';
            matrix[6, 7] = 'X'; matrix[6, 8] = 'X'; matrix[6, 9] = 'X';
            matrix[7, 0] = 'X'; matrix[7, 1] = 'X'; matrix[7, 2] = 'X'; matrix[7, 3] = 'X'; matrix[7, 4] = 'X'; matrix[7, 5] = 'X'; matrix[7, 6] = 'X';
            matrix[7, 7] = 'X'; matrix[7, 8] = 'X'; matrix[7, 9] = 'X';
            matrix[8, 0] = 'O'; matrix[8, 1] = 'X'; matrix[8, 2] = 'O'; matrix[8, 3] = 'X'; matrix[8, 4] = 'X'; matrix[8, 5] = 'X'; matrix[8, 6] = 'X';
            matrix[8, 7] = 'X'; matrix[8, 8] = 'X'; matrix[8, 9] = 'X';
            matrix[9, 0] = 'X'; matrix[9, 1] = 'X'; matrix[9, 2] = 'X'; matrix[9, 3] = 'X'; matrix[9, 4] = 'X'; matrix[9, 5] = 'X'; matrix[9, 6] = 'X';
            matrix[9, 7] = 'O'; matrix[9, 8] = 'O'; matrix[9, 9] = 'O';

            Console.WriteLine("  1  2  3  4  5  6  7  8  9  10");
            Console.WriteLine("А\nБ\nВ\nГ\nД\nЕ\nЁ\nЖ\nЗ\nИ\nК\n");

            for (int i = 0; i < matrix.GetLength(0); i++)
            {
                for (int j = 0; j < matrix.GetLength(1); j++)
                {
                    Console.Write($"  {matrix[i, j]}");
                }
                Console.WriteLine();
            }

            Console.ReadLine();
        }
    }
}
