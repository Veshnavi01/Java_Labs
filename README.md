[Program-1 Program to add two distances given in m, mm and cm](#Assi-1) 

[Program-2 Program to add two distances given in km and m](#Assi-2)

[Program-3 Program to print multiples of input values](#Assi-3)

[Program-4 Program to perform 5 arithmetic operations](#Assi-4)

[Program-5 5 C language programs in java: Armstrong, Palindrome, Fibonacci Series, Factorial, Pattern](#Assi-5)

[Program-6 Program to add two times given in hrs, min and sec](#Assi-6)

[Program-7 Program to add two times given in hrs and min](#Assi-7)

[Program-8 Program to reverse a given number using 4 functions: input, idisplay, reverse, revdisplay](#Assi-8)

[Program-9 Program to do matrix operations](#Assi-9)

[Program-10 Program using 3 classes to print 1-100, 3 times with and without thread and analyse it's output. And repeat the same program using runnable interface.](#Assi-10)

[Program-11 Using the concept of multithreading the output of these threads is unpredictable and all the threads must be synchronised, use join method.](#Assi-11)

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

public class Distance {
    public static void main(String[] args){
        Adddistance o1 = new Adddistance();
        Adddistance o2 = new Adddistance();
        Adddistance o3 = new Adddistance();
        o1.input();
        o2.input();
        o3.add(o1,o2);
        o3.output();    
    }
    
}


class Adddistance{
    int m;
    int km;
    
    void input(){
        Scanner sc1 =  new Scanner(System.in);
        System.out.println("Enter the distance in km:");
        km = sc1.nextInt();
        Scanner sc2 =  new Scanner(System.in);
        System.out.println("Enter the distance in m:");
        m = sc2.nextInt();
       
        
    }
    void output(){
       System.out.println("Total Distance = "+km+"km"+m+"m");
      
    }
    void add(Adddistance d1,Adddistance d2){
        km = d1.km+d2.km;
        m = d1.m+d2.m;
        if(m >= 1000){
            km+=1;
            m = m-1000;
        }
        
    }
}
```
<img width="381" height="321" alt="image" src="https://github.com/user-attachments/assets/a099960d-3671-4673-8ed4-80dc1525c705" />


## Assi-3
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

## Assi-4
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


## Assi-5
```
import java.util.Scanner;
public class Fivefunctions {
    
    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);
        Scanner sc1 = new Scanner(System.in);
        Scanner sc2 = new Scanner(System.in);
        Scanner sc3 = new Scanner(System.in);
        Scanner sc4 = new Scanner(System.in);
        Scanner sc5 = new Scanner(System.in);
        
        System.out.print("Enter a number to check Armstrong: ");
        int n = sc.nextInt();
        Armstrong obj = new Armstrong(n); 
        obj.check(); 
        
        System.out.print("Enter a number to check Palindrome: ");
        int n1 = sc1.nextInt();
        PalindromeNumber p1 = new PalindromeNumber(n1);
        p1.check();
        
        System.out.print("Enter a number to find it's factorial: ");
        int n2 = sc2.nextInt();
        FactorialNumber Num1 = new FactorialNumber(n2);
        Num1.calculate();

        System.out.print("Enter number of terms to print fibonacci series: ");
        int num = sc3.nextInt();
        FibonacciSeries fib = new FibonacciSeries(num);
        fib.printSeries(); 
        
        System.out.println("Enter number of rows and columns to print square pattern: ");
        int n4 = sc4.nextInt();
        int n5 = sc5.nextInt();
        Pattern pa = new Pattern(n4,n5);
        pa.display();
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

        System.out.println("Fibonacci Series: ");

        for (int i = 1; i <= n; i++) {
            System.out.print(a + " ");
            c = a + b;
            a = b;
            b = c;
        }
        System.out.println();
    }
}

class Pattern{
    int r,c;
    
    Pattern(int r, int c){
        this.r = r;
        this.c = c;
    }
    
    void display(){
        
        for(int i = 0; i<r; i++){
            for(int j = 0; j<c; j++){
                System.out.print("* ");
            }
            System.out.println();
        }
    }
}
```
<img width="576" height="483" alt="image" src="https://github.com/user-attachments/assets/3b72be99-b1d1-4b64-a121-935e1e8ea52d" />

## Assi-6
```
import java.util.Scanner;

public class Time {
     public static void main(String[] args) {
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
    int hr;
    int min;
    int sec;
    
    void input(){
        Scanner sc1 =  new Scanner(System.in);
        System.out.println("Enter the time in hr:");
        hr = sc1.nextInt();
        Scanner sc2 =  new Scanner(System.in);
        System.out.println("Enter the time in min:");
        min = sc2.nextInt();
        Scanner sc3 =  new Scanner(System.in);
        System.out.println("Enter the time in sec:");
        sec = sc3.nextInt();
        
    }
    void output(){
       System.out.println("Total time = "+hr+"hr"+min+"min"+sec+"sec");
    }
    void add(Test1 t1,Test1 t2){
        hr = t1.hr+t2.hr;
        min = t1.min+t2.min;
        sec = t1.sec+t2.sec;
        if(sec >= 60){
            min+=1;
            sec = sec-60;
        }
        if(min >= 60){
            hr+=1;
            min = min-60;
        }
        
    }
}
```
<img width="401" height="407" alt="image" src="https://github.com/user-attachments/assets/0eaea47c-8eda-4f6f-8c77-7e7636c0ef1d" />

## Assi-7
```
import java.util.Scanner;

public class Time {
     public static void main(String[] args) {
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
    int hr;
    int min;
    
    void input(){
        Scanner sc1 =  new Scanner(System.in);
        System.out.println("Enter the time in hr:");
        hr = sc1.nextInt();
        Scanner sc2 =  new Scanner(System.in);
        System.out.println("Enter the time in min:");
        min = sc2.nextInt();
        
    }
    void output(){
       System.out.println("Total time = "+hr+"hr"+min+"min");
    }
    void add(Test1 t1,Test1 t2){
        hr = t1.hr+t2.hr;
        min = t1.min+t2.min;
        if(min >= 60){
            hr+=1;
            min = min-60;
        }
        
    }
}
```
<img width="381" height="320" alt="image" src="https://github.com/user-attachments/assets/0edd9a3d-8e75-43c6-8314-fdced7dc6be1" />

## Assi-8
```
import java.util.Scanner;

public class Reversing {
    public static void main(String[] args){
        
        Reverse o1 = new Reverse();
        o1.input();
        o1.idisplay();
        o1.reverse();
        o1.revdisplay();
        
       
    }
}

class Reverse{
    int n;
    int result;
    
    void idisplay(){
        System.out.println("Original number = "+n);
    }
    
    void input(){
        Scanner sc = new Scanner(System.in);
        System.out.println("Enter a number:");
        n = sc.nextInt();
    }
    
    void reverse(){
        int rem;
        result = 0;
        while(n>0){
        rem = n%10;
        result = result*10 + rem;
        n = n/10;
        }
    }
        
     void revdisplay(){
        System.out.println("Reversed Number = "+result);
    }   
}
```
<img width="296" height="90" alt="image" src="https://github.com/user-attachments/assets/7f7f2e0c-da89-4091-9c69-812c7d839b02" />

## Assi-9
```
import java.util.Scanner;
public class MatrixOperations {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int rows, cols;
        // Input matrix size
        System.out.print("Enter number of rows: ");
        rows = sc.nextInt();
        System.out.print("Enter number of columns: ");
        cols = sc.nextInt();
        int[][] A = new int[rows][cols];
        int[][] B = new int[rows][cols];
        // Input Matrix A
        System.out.println("Enter elements of Matrix A:");
        for (int i = 0; i < rows; i++) {
            for (int j = 0; j < cols; j++) {
                A[i][j] = sc.nextInt();
            }
        }
        // Input Matrix B
        System.out.println("Enter elements of Matrix B:");
        for (int i = 0; i < rows; i++) {
            for (int j = 0; j < cols; j++) {
                B[i][j] = sc.nextInt();
            }
        }
        // Matrix Addition
        int[][] sum = new int[rows][cols];
        System.out.println("\nMatrix Addition:");
        for (int i = 0; i < rows; i++) {
            for (int j = 0; j < cols; j++) {
                sum[i][j] = A[i][j] + B[i][j];
                System.out.print(sum[i][j] + " ");
            }
            System.out.println();
        }
        // Transpose of Matrix A
        System.out.println("\nTranspose of Matrix A:");
        for (int i = 0; i < cols; i++) {
            for (int j = 0; j < rows; j++) {
                System.out.print(A[j][i] + " ");
            }
            System.out.println();
        }
        // Sum of Rows (Matrix A)
        System.out.println("\nSum of each row (Matrix A):");
        for (int i = 0; i < rows; i++) {
            int rowSum = 0;
            for (int j = 0; j < cols; j++) {
                rowSum += A[i][j];
            }
            System.out.println("Row " + (i + 1) + " sum = " + rowSum);
        }
        // Sum of Columns (Matrix A)
        System.out.println("\nSum of each column (Matrix A):");
        for (int j = 0; j < cols; j++) {
            int colSum = 0;
            for (int i = 0; i < rows; i++) {
                colSum += A[i][j];
            }
            System.out.println("Column " + (j + 1) + " sum = " + colSum);
        }
        // Sum of Diagonals (Matrix A)
        if (rows == cols) {
            int primaryDiagonal = 0, secondaryDiagonal = 0;

            for (int i = 0; i < rows; i++) {
                primaryDiagonal += A[i][i];
                secondaryDiagonal += A[i][rows - i - 1];
            }
            System.out.println("\nPrimary diagonal sum = " + primaryDiagonal);
            System.out.println("Secondary diagonal sum = " + secondaryDiagonal);
        } else {
            System.out.println("\nDiagonal sums not possible (Matrix is not square).");
        }
        sc.close();
    }
}
```
<img width="323" height="526" alt="image" src="https://github.com/user-attachments/assets/b3431eb1-5b9a-4e65-8cf5-9c6310763100" />
<img width="362" height="255" alt="image" src="https://github.com/user-attachments/assets/413fdd1a-982d-49b0-94f9-6a9ecf42b4bc" />

## Assi-10
```
public class Main {
    public static void main(String[] args){
        Student1 s1 = new Student1();
        Student2 s2 = new Student2();
        Student3 s3 = new Student3();
        
        s1.fun();
        s2.fun();
        s3.fun();
    }
}

class Student1{
        
        void fun(){
            for(int i=1; i<=100; i++){
                System.out.println("Student1 : "+ i);
            }
        }
} 
class Student2{
        
        void fun(){
            for(int i=1; i<=100; i++){
                System.out.println("Student2 : "+ i);
            }
        }
} 
class Student3{
        
        void fun(){
            for(int i=1; i<=100; i++){
                System.out.println("Student3 : "+ i);
            }
        }
} 
```
<img width="141" height="789" alt="image" src="https://github.com/user-attachments/assets/b99d9260-57d0-4da6-8cbd-f0cfbea91842" />
<img width="139" height="709" alt="image" src="https://github.com/user-attachments/assets/f2a22504-1227-4097-a694-5a6e6b103fde" />
<img width="142" height="772" alt="image" src="https://github.com/user-attachments/assets/b21eb629-ad36-48b9-9175-1bb9d5dac44d" />
<img width="131" height="770" alt="image" src="https://github.com/user-attachments/assets/07ede5c9-291c-45ad-9d4b-c0423a7d016e" />
<img width="129" height="773" alt="image" src="https://github.com/user-attachments/assets/2c8a46eb-e6d3-457a-a3bd-539abd981f5d" />
<img width="142" height="774" alt="image" src="https://github.com/user-attachments/assets/db3333a9-3081-4c38-aa75-4b32bca78fea" />
<img width="139" height="774" alt="image" src="https://github.com/user-attachments/assets/8884da39-6bc8-4d5a-a3dd-62714caaab86" />
<img width="135" height="774" alt="image" src="https://github.com/user-attachments/assets/9ad5b84e-6b5d-4230-8139-893e9a58822e" />
<img width="366" height="437" alt="image" src="https://github.com/user-attachments/assets/e0e04a74-adaa-45cb-ae74-36b927bccf3a" />

```
public class Test {
    public static void main(String[] args){
        Student1th s1 = new Student1th();
        Student2th s2 = new Student2th();
        Student3th s3 = new Student3th();
        
        s1.start();
        s2.start();
        s3.start();
    }
}

class Student1th extends Thread{
        
        public void run(){
            for(int i=1; i<=100; i++){
                System.out.println("Student1 : "+ i);
            }
        }
} 
class Student2th extends Thread{
        
        public void run(){
            for(int i=1; i<=100; i++){
                System.out.println("Student2 : "+ i);
            }
        }
} 
class Student3th extends Thread{
        
        public void run(){
            for(int i=1; i<=100; i++){
                System.out.println("Student3 : "+ i);
            }
        }
} 
```
<img width="143" height="794" alt="image" src="https://github.com/user-attachments/assets/a026b16f-92a1-4941-8dbb-44ede8b24f87" />
<img width="140" height="768" alt="image" src="https://github.com/user-attachments/assets/6a0727d0-4500-4b63-afbb-0b230400763a" />
<img width="139" height="770" alt="image" src="https://github.com/user-attachments/assets/1cd9506f-5ba6-4007-bb3c-bd3d9bed68f0" />
<img width="152" height="768" alt="image" src="https://github.com/user-attachments/assets/10274b5f-f3a3-4449-87a6-f293adab2fcd" />
<img width="146" height="770" alt="image" src="https://github.com/user-attachments/assets/77a995d8-a914-48be-aee1-78db1aea2552" />
<img width="131" height="766" alt="image" src="https://github.com/user-attachments/assets/4776176f-1f65-4f5b-b4fb-b50f8adeafc7" />
<img width="139" height="776" alt="image" src="https://github.com/user-attachments/assets/39960b1b-a124-41f4-9324-a782dbb6c63c" />
<img width="139" height="770" alt="image" src="https://github.com/user-attachments/assets/c06e9bf7-9320-49f2-9cec-2f008acac330" />
<img width="365" height="375" alt="image" src="https://github.com/user-attachments/assets/351d994d-5028-4578-9a11-eda89668640f" />

```
public class New {
    public static void main(String[] args){
        th1 s1 = new th1();
        th2 s2 = new th2();
        th3 s3 = new th3();
        
        Thread h1 = new Thread(s1);
        Thread h2 = new Thread(s2);
        Thread h3 = new Thread(s3);
        
        h1.start();
        h2.start();
        h3.start();
    }
}
class th1 implements Runnable{
        
        public void run(){
            for(int i=1; i<=100; i++){
                System.out.println("Student1 : "+ i);
            }
        }
} 
class th2 implements Runnable{
        
        public void run(){
            for(int i=1; i<=100; i++){
                System.out.println("Student2 : "+ i);
            }
        }
} 
class th3 implements Runnable{
        
        public void run(){
            for(int i=1; i<=100; i++){
                System.out.println("Student3 : "+ i);
            }
        }
}
```
<img width="144" height="790" alt="image" src="https://github.com/user-attachments/assets/57d4b302-bfb2-4775-8c9c-dc63aaabdb5c" />
<img width="139" height="790" alt="image" src="https://github.com/user-attachments/assets/4f5b52a8-918e-48ee-9c8e-ec10cd3dd062" />
<img width="145" height="769" alt="image" src="https://github.com/user-attachments/assets/a5860fd3-982c-484d-8f02-54d2f78244ae" />
<img width="145" height="775" alt="image" src="https://github.com/user-attachments/assets/f94d28cd-24e3-4f16-a741-7d0379c4cee8" />
<img width="144" height="769" alt="image" src="https://github.com/user-attachments/assets/dd3a0611-2593-48b0-88c6-ce5567bc9c28" />
<img width="133" height="773" alt="image" src="https://github.com/user-attachments/assets/86fa2b85-2e04-456c-9b4f-b8b5362c0477" />
<img width="134" height="776" alt="image" src="https://github.com/user-attachments/assets/67f110e6-a2e4-4103-beb8-514d931f5a96" />
<img width="134" height="768" alt="image" src="https://github.com/user-attachments/assets/2331abe7-fad0-4a75-91d3-d3a9abca5dbc" />
<img width="361" height="432" alt="image" src="https://github.com/user-attachments/assets/4f7c442c-18c5-4c2c-8de0-75cea4c32c9c" />

## Assi-11
```

```






