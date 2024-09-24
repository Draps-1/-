Задание №6
using System;

class Program {
    static void Main(string[] args) {
        int n = int.Parse(Console.ReadLine());
        int[] arr = Array.ConvertAll(Console.ReadLine().Split(), int.Parse);

        // Циклический сдвиг вправо
        int temp = arr[n - 1];
        for (int i = n - 1; i > 0; i--) {
            arr[i] = arr[i - 1];
        }
        arr[0] = temp;

        Console.WriteLine(string.Join(" ", arr));
    }
}


Задание №4
using System;

class Program {
    static void Main(string[] args) {
        // Считываем кол-во элементов в массиве
        int n = int.Parse(Console.ReadLine());

        // Считываем элементы массива и преобразуем их в целочисленный массив
        int[] arr = Array.ConvertAll(Console.ReadLine().Split(), int.Parse);

        int distinctCount = 1;

        // Проходим по массиву, начиная со второго элемента
        for (int i = 1; i < n; i++) {
            // Если текущий элемент отличается от предыдущего,
            // увеличиваем счетчик количества различных элементов
            if (arr[i] != arr[i - 1]) {
                distinctCount++;
            }
        }

        // Выводим результат
        Console.WriteLine(distinctCount);
    }
}



Задание №1
using System;

class Program {
    static void Main(string[] args) {
        // Считываем количество элементов в массиве
        int n = int.Parse(Console.ReadLine());

        // Считываем элементы массива и преобразуем их в целочисленный массив
        int[] arr = Array.ConvertAll(Console.ReadLine().Split(), int.Parse);

        // Выводим элементы, которые больше предыдущего
        for (int i = 1; i < n; i++) {
            if (arr[i] > arr[i - 1]) {
                Console.Write(arr[i] + " ");
            }
        }
    }
}
