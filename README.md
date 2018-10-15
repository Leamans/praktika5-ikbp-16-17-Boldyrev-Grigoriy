# praktika5-ikbo-16-17-Boldyrev-Grigoriy

# Вариант 1

public class Main {

    public static void practFunc(int number)
    {
        if(number != 0)
        {
            boolean key = false;
            for (int index = number; index >= 1; index--)
            {
                if(key == false)
                {
                    practFunc(number-1);
                    key = true;
                }
                System.out.print(number + ", ");
            }
        }
    }

    public static void main(String[] args) {
        int number = 4;
        practFunc(number);
    }
}
