namespace LinearSearchFruitsTask
{
    internal class Program
    {
        static void Main(string[] args)
        {
            string[] fruits = { "banana", "apple", "orange", "pear", "grape", "pineapple" };

            Console.Write("Enter a word to search for: ");
            string userSearch = Console.ReadLine();

            bool isFound = false;
            
            for (int i = 0; i < fruits.Length; i++)
            {
                if (fruits[i] == userSearch)
                {
                    isFound = true;
                    break;
                }
            }

            Console.WriteLine(isFound);
        }
    }
}
