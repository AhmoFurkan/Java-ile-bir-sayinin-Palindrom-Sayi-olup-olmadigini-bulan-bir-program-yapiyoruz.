# Java-ile-bir-sayinin-Palindrom-Sayi-olup-olmadigini-bulan-bir-program-yapiyoruz.
Palindromik sayı, iki taraftan okunduğu zaman okunuş yönüyle aynı olan sayılardır.


    public class Main {

    static boolean isPalindrom(int number) {
        int temp = number, reverseNumber = 0, lastNumber;
        while (temp != 0) {
            lastNumber = temp % 10;
            reverseNumber = (reverseNumber * 10) + lastNumber;
            temp /= 10;

        }
        if (number==reverseNumber)
             return true;
        else
            return false;
    }

    public static void main(String[] args) {
        System.out.println(isPalindrom(4004));
     }
    }
    
![image](https://user-images.githubusercontent.com/107626332/183841545-0dc8a4a7-4b77-41e0-ab66-0bf47f0c62b1.png)
https://app.patika.dev/ahmetfurkan
