[Program-1 Program to add two distances](#Assi-1) 

[Program-2 Program to print multiples of input values](#Assi-2)

[Program-3 Program to make a calculator](#Assi-3)

[Program-4 Program to check whether a number is armstrong number or not](#Assi-4)

[Program-5 Program to check whether a number is palindrome or not](#Assi-5)

[Program-6 Program to print the factorial of a given number](#Assi-6)

[Program-7 Program to print fibbonacci series](#Assi-7)

## Assi-1
```
import java.util.Scanner;

public class distance {
    public static void main(String[] args){
        Test1 o1 = new Test1();
        Test1 o2 = new Test1();
        Test1 o3 = new Test1();
        o1.input();
        o2.input();
        o3.add(o1,o2);
        o3.output();    
    }
}

class Test1{
    int m;
    int mm;
    int cm;
    
    void input(){
        Scanner sc1 =  new Scanner(System.in);
        System.out.println("Enter the distance in m:");
        m = sc1.nextInt();
        Scanner sc2 =  new Scanner(System.in);
        System.out.println("Enter the distance in cm:");
        cm = sc2.nextInt();
        Scanner sc3 =  new Scanner(System.in);
        System.out.println("Enter the distance in mm:");
        mm = sc3.nextInt();
        
    }
    void output(){
       System.out.println("Distance in m = "+m);
       System.out.println("Distance in cm = "+cm);
       System.out.println("Distance in mm = "+mm);
    }
    void add(Test1 d1,Test1 d2){
        m = d1.m+d2.m;
        cm = d1.cm+d2.cm;
        mm = d1.mm+d2.mm;
        if(mm >= 10){
            cm+=1;
            mm = mm-10;
        }
        if(cm >= 100){
            m+=1;
            cm = cm-100;
        }
        
    }
}
```

<img width="297" height="350" alt="image" src="https://github.com/user-attachments/assets/314192a2-0392-45e9-bc90-1ae71120f885" />

## Assi-2
```
import java.util.Scanner;

public class veshnavi {
    public static void main(String[] args) {
        System.out.println("Hello");
        Test t1 = new Test();
        
        t1.input();
        t1.proc();
        t1.output();
    }
    
}
class Test {
    int a;
    int b;
    int c;
    
    void input()
    {
        Scanner s1= new Scanner(System.in);
        System.out.println("Enter the value of a:");
        a = s1.nextInt();
        Scanner s2= new Scanner(System.in);
        System.out.println("Enter the value of b:");
        b = s2.nextInt();
        Scanner s3= new Scanner(System.in);
        System.out.println("Enter the value of c:");
        c = s3.nextInt();
    }
    void output()
    {
        System.out.println("a ="+a);
        System.out.println("b ="+b);
        System.out.println("c ="+c);
    }
    void proc()
    {
        a = a*2;
        b = b*3;
    }
}
```
<img width="302" height="266" alt="image" src="https://github.com/user-attachments/assets/852a9dd8-8e0f-461a-a6d2-f8851c982208" />

## Assi-3
```
public class Calculator {
    void add(int a, int b) {
        System.out.println("Addition = " + (a+b));
    }  

    void subtract(int a, int b) {
        System.out.println("Subtraction = " + (a-b));
    }

    void multiply(int a, int b) {
        System.out.println("Multiplication = " + (a*b));
    }

    void divide(double a, double b) {
        System.out.println("Division = " + (a/b));
    }

    void modulo(int a, int b) {
        System.out.println("Modulo = " + (a%b));
    }
    public static void main(String[] args) {
            Calculator c1 = new Calculator();
            c1.add(5,3);
            c1.subtract(5,3);
            c1.multiply(5,3);
            c1.divide(5,3);
            c1.modulo(5,3);
        }
    }
  ```
<img width="294" height="193" alt="image" src="https://github.com/user-attachments/assets/0cc23c87-1a89-4d4a-ae23-50e2e485c086" />


## Assi-4
```
import java.util.Scanner;
public class ArmstrongNumber {
    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);
        System.out.print("Enter a number: ");
        int n = sc.nextInt();

        Armstrong obj = new Armstrong(n); 
        obj.check(); 
    }
}
    
    

class Armstrong {

    int num;
    
    Armstrong(int n) {
        num = n;
    }
    
    void check() {
        int original = num;
        int remainder;
        int result = 0;

        while (num != 0) {
            remainder = num % 10;
            result = result + (remainder * remainder * remainder);
            num = num / 10;
        }

        if (result == original) {
            System.out.println(original + " is an Armstrong number");
        } else {
            System.out.println(original + " is not an Armstrong number");
        }
    }
}
```
<img width="323" height="137" alt="image" src="https://github.com/user-attachments/assets/b692f321-b170-474b-a42b-abe2b1a5d0b8" />
<img width="294" height="136" alt="image" src="https://github.com/user-attachments/assets/9fdc9b74-b0b8-465d-a386-dc66e77bf3cf" />

## Assi-5
```
import java.util.Scanner;
public class Palindrome {
    public static void main(String[]args){
        
        Scanner sc = new Scanner(System.in);
        System.out.println("Enter the number:");
        int n = sc.nextInt();
        
        PalindromeNumber p1 = new PalindromeNumber(n);
        p1.check();
    } 
}
class PalindromeNumber{
    
    int num,num1;
    int result = 0;
    int remainder;
    
    PalindromeNumber(int n)
    {
        num = n;
    }
    
    void check()
    {
        num1 = num;
        while(num1!=0){
            remainder = num1%10;
            result = (result*10)+remainder;
            num1 = num1/10;
        }
        if(result == num){
            System.out.println("The number is palindromic");
        }
        else{
             System.out.println("The number is not a palindromic number");
        }
    }
}
```
<img width="325" height="166" alt="image" src="https://github.com/user-attachments/assets/d48e6de4-b519-4636-9fba-0d96da87fa23" />
<img width="297" height="154" alt="image" src="https://github.com/user-attachments/assets/80a75505-d739-405d-8fae-d09dfd490697" />


## Assi-6
```
import java.util.Scanner;

public class Factorial {
    public static void main(String[]args){
        
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter a number:");
        int n = sc.nextInt();
        
        FactorialNumber Num1 = new FactorialNumber(n);
        Num1.calculate();
        
    }
}

class FactorialNumber{
    
    int num;
    int result = 1;
    FactorialNumber(int n){
        num = n;
    }
    
    void calculate(){
        while(num!=0){
            result*=num;
            num = num-1;
        }
        System.out.println("Factorial = "+result);
    }
}
```
<img width="291" height="140" alt="image" src="https://github.com/user-attachments/assets/e065c569-c616-43e9-b06a-4df445d2307b" />

## Assi-7
```
import java.util.Scanner;

public class Fibonacci {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter number of terms: ");
        int num = sc.nextInt();

        FibonacciSeries obj = new FibonacciSeries(num); // object creation
        obj.printSeries(); // method call
    }
    
}

class FibonacciSeries {
    int n;

    // Constructor
    FibonacciSeries(int n) {
        this.n = n;
    }

    // print Fibonacci series
    void printSeries() {
        int a = 0;
        int b = 1;
        int c;

        System.out.print("Fibonacci Series: ");

        for (int i = 1; i <= n; i++) {
            System.out.print(a + " ");
            c = a + b;
            a = b;
            b = c;
        }
    }
}
```
<img width="294" height="139" alt="image" src="https://github.com/user-attachments/assets/dfa15769-4e44-40c4-9ee1-216d11432b57" />















