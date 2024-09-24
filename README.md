Задание №6:


система;

программа класса {
    static void Main(string[] args) {
        int n = int.Parse(Console.ReadLine());
        int[] arr = Array.ConvertAll(Console.ReadLine().Split(), int.Parse);

        // Циклический поворот вправо
        int temp = arr[n - 1];
        for (int i = n - 1; i &gt; 0; i--) {
            доход[я] = доход[я - 1];
        }
        arr[0] = температура;

        Console.WriteLine(string.Join(" ", arr));
    }
}


Задание №4:


используя систему;

программа класса {
    static void Main(string[] args) {
        // Считываем кол-во элементов в массиве
        int n = int.Parse(Console.ReadLine());

        // Считываем элементы массива и преобразуем их в целочисленный массив.
        int[] arr = Array.ConvertAll(Console.ReadLine().Split(), int.Parse);

        int DifferentCount = 1;

        // Проходим по массиву, начиная со второго элемента
        для (int i = 1; я &lt; n; я++) {
            // Если какой-либо элемент отличается от внешнего вида,
            // увеличиваем счетчик количества различных элементов
            если (arr[i] != arr[i - 1]) {
                DifferentCount++;
            }
        }

        // Выводим результат
        Console.WriteLine(distinctCount);
    }
}



Задание №1:


используя систему;

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
