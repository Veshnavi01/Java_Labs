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

[Program-11 Using the concept of multithreading the output of these threads is unpredictable and all the threads must be synchronised (use join method).](#Assi-11)

[Program-12 Write a program for addition of 2 numbers using swing.](#Assi-12)

[Program-13 Inheritance Programs, using interface and abstract classes.](#Assi-13)

[Program-14 Make one calculator in swing.](#Assi-14)

[Program-15 Matrix Addition using swing class.](#Assi-15)

[Program-16  Create one jframe apply 10 buttons on that after clicking on each button a new
structure is created.(Circle, oval rectangle, etc ....).](#Assi-16)

[Program-17 Just using mouse Event create a frame like paint brush with selection of colour and width.](#Assi-17)

[Program-18 Create a package of any 5 classes of your choice and import it.](#Assi-18)

[Program-19 Create one package and sub package  import and test it.](#Assi-19)

[Program-20 Create one small array of size 5 apply array out of bounds exception using try catch give a proper message in catch and demonstrate the exception exactly in the same fashion demonstrate arithmetic exception.](#Assi-20)

[Program-21 To test the range of age of one student.write a program using user defined exception.](#Assi-21)

[Program-22 File Handling Programs (given in the PPT).](#Assi-22)

[Program-23 5 programs using java data structures.](#Assi-23)


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
public class Test {
    public static void main(String[] args) {
        Student1th s1 = new Student1th();
        Student2th s2 = new Student2th();
        Student3th s3 = new Student3th();

        try {
            s1.start();
            s1.join();   // wait until s1 finishes

            s2.start();
            s2.join();   // wait until s2 finishes

            s3.start();
            s3.join();   // wait until s3 finishes
        } catch (InterruptedException e) {
            System.out.println(e);
        }
    }
}

class Student1th extends Thread {
    public void run() {
        for (int i = 1; i <= 100; i++) {
            System.out.println("Student1 : " + i);
        }
    }
}

class Student2th extends Thread {
    public void run() {
        for (int i = 1; i <= 100; i++) {
            System.out.println("Student2 : " + i);
        }
    }
}

class Student3th extends Thread {
    public void run() {
        for (int i = 1; i <= 100; i++) {
            System.out.println("Student3 : " + i);
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


## Assi-12
```
import javax.swing.*;

public class Add {
    public static void main(String[] args) {
        JFrame f = new JFrame("Addition");

        JLabel l1 = new JLabel("Enter Number 1:");
        JLabel l2 = new JLabel("Enter Number 2:");
        JLabel l3 = new JLabel("Result:");

        JTextField t1 = new JTextField();
        JTextField t2 = new JTextField();
        JTextField t3 = new JTextField();

        JButton b = new JButton("Add");

        l1.setBounds(30, 30, 120, 30);
        t1.setBounds(160, 30, 100, 30);

        l2.setBounds(30, 70, 120, 30);
        t2.setBounds(160, 70, 100, 30);

        b.setBounds(90, 110, 80, 30);

        l3.setBounds(30, 150, 120, 30);
        t3.setBounds(160, 150, 100, 30);

        f.add(l1); 
        f.add(t1);
        f.add(l2); 
        f.add(t2);
        f.add(b);
        f.add(l3); 
        f.add(t3);

        // Button action
        b.addActionListener(e -> {
            int a = Integer.parseInt(t1.getText());
            int b1 = Integer.parseInt(t2.getText());
            t3.setText(String.valueOf(a + b1));
        });

        f.setSize(320, 250);
        f.setLayout(null);
        f.setVisible(true);
        f.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
    }
}
```
<img width="230" height="182" alt="image" src="https://github.com/user-attachments/assets/8e392859-97c8-450f-bd82-8516c6a645ac" />


## Assi-13
```
interface Shape {
    void area();
}

class Rectangle implements Shape {
    int length = 10, breadth = 5;

    public void area() {
        System.out.println("Area of Rectangle = " + (length * breadth));
    }
}

class Circle implements Shape {
    int radius = 7;

    public void area() {
        System.out.println("Area of Circle = " + (3.14 * radius * radius));
    }
}

public class InterfaceInheritance {
    public static void main(String[] args) {
        Rectangle r = new Rectangle();
        Circle c = new Circle();

        r.area();
        c.area();
    }
}
```
<img width="558" height="91" alt="image" src="https://github.com/user-attachments/assets/88cd740c-fafe-4934-afe4-2faf8d23e518" />

```
abstract class Shape {
    abstract void area();

    void display() {
        System.out.println("Calculating Area...");
    }
}

class Rectangle extends Shape {
    int length = 10, breadth = 5;

    void area() {
        System.out.println("Area of Rectangle = " + (length * breadth));
    }
}

class Circle extends Shape {
    int radius = 7;

    void area() {
        System.out.println("Area of Circle = " + (3.14 * radius * radius));
    }
}

public class AbstractInheritance {
    public static void main(String[] args) {
        Rectangle r = new Rectangle();
        Circle c = new Circle();

        r.display();
        r.area();

        c.display();
        c.area();
    }
}
```
<img width="553" height="90" alt="image" src="https://github.com/user-attachments/assets/66439441-92a8-4bf7-aeb8-3f69a56f3c72" />

## Assi-14
```
import javax.swing.*;
import java.awt.event.*;

public class Calculator {
    public static void main(String[] args) {
        JFrame f = new JFrame("Calculator");

        JLabel l1 = new JLabel("Enter Number 1:");
        JLabel l2 = new JLabel("Enter Number 2:");
        JLabel l3 = new JLabel("Result:");

        JTextField t1 = new JTextField();
        JTextField t2 = new JTextField();
        JTextField t3 = new JTextField();

        JButton add = new JButton("+");
        JButton sub = new JButton("-");
        JButton mul = new JButton("*");
        JButton div = new JButton("/");

        l1.setBounds(30, 30, 120, 30);
        t1.setBounds(160, 30, 100, 30);

        l2.setBounds(30, 70, 120, 30);
        t2.setBounds(160, 70, 100, 30);

        l3.setBounds(30, 110, 120, 30);
        t3.setBounds(160, 110, 100, 30);

        add.setBounds(30, 160, 50, 30);
        sub.setBounds(90, 160, 50, 30);
        mul.setBounds(150, 160, 50, 30);
        div.setBounds(210, 160, 50, 30);

        f.add(l1); f.add(t1);
        f.add(l2); f.add(t2);
        f.add(l3); f.add(t3);

        f.add(add); f.add(sub); f.add(mul); f.add(div);

        add.addActionListener(e -> {
            int a = Integer.parseInt(t1.getText());
            int b = Integer.parseInt(t2.getText());
            t3.setText(String.valueOf(a + b));
        });

        sub.addActionListener(e -> {
            int a = Integer.parseInt(t1.getText());
            int b = Integer.parseInt(t2.getText());
            t3.setText(String.valueOf(a - b));
        });

        mul.addActionListener(e -> {
            int a = Integer.parseInt(t1.getText());
            int b = Integer.parseInt(t2.getText());
            t3.setText(String.valueOf(a * b));
        });

        div.addActionListener(e -> {
            int a = Integer.parseInt(t1.getText());
            int b = Integer.parseInt(t2.getText());
            t3.setText(String.valueOf(a / b));
        });

        f.setSize(320, 250);
        f.setLayout(null);
        f.setVisible(true);
        f.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
    }
}
```
<img width="231" height="182" alt="image" src="https://github.com/user-attachments/assets/48fa72ad-d99b-4c45-9d39-924efdb1e7e6" />
<img width="232" height="181" alt="image" src="https://github.com/user-attachments/assets/12e157d3-49a3-4978-808a-82dc3eac11ef" />
<img width="229" height="181" alt="image" src="https://github.com/user-attachments/assets/9c3e921c-3733-4e55-be64-2c3b11b340e4" />
<img width="230" height="179" alt="image" src="https://github.com/user-attachments/assets/0bf70cd8-b731-4f19-be3e-9b7d1fb84933" />



## Assi-15
```
import javax.swing.*;
import java.awt.event.*;

public class MatrixAdd {
    public static void main(String[] args) {

        JFrame f = new JFrame("Dynamic Matrix Addition");

        JLabel sizeLabel = new JLabel("Enter Size:");
        JTextField sizeField = new JTextField();
        JButton create = new JButton("Create Matrix");

        sizeLabel.setBounds(50, 20, 100, 30);
        sizeField.setBounds(150, 20, 50, 30);
        create.setBounds(220, 20, 130, 30);

        f.add(sizeLabel);
        f.add(sizeField);
        f.add(create);

        create.addActionListener(e -> {
            int n = Integer.parseInt(sizeField.getText());

            JTextField[][] A = new JTextField[n][n];
            JTextField[][] B = new JTextField[n][n];
            JTextField[][] C = new JTextField[n][n];

            JLabel l1 = new JLabel("Matrix A");
            JLabel l2 = new JLabel("Matrix B");
            JLabel l3 = new JLabel("Result");

            l1.setBounds(50, 70, 100, 20);
            l2.setBounds(250, 70, 100, 20);
            l3.setBounds(450, 70, 100, 20);

            f.add(l1); f.add(l2); f.add(l3);

            int x = 50, y = 100;

            for(int i=0;i<n;i++){
                for(int j=0;j<n;j++){
                    A[i][j] = new JTextField();
                    A[i][j].setBounds(x + j*50, y + i*40, 40, 30);
                    f.add(A[i][j]);
                }
            }

            x = 250;
            for(int i=0;i<n;i++){
                for(int j=0;j<n;j++){
                    B[i][j] = new JTextField();
                    B[i][j].setBounds(x + j*50, y + i*40, 40, 30);
                    f.add(B[i][j]);
                }
            }
            
            x = 450;
            for(int i=0;i<n;i++){
                for(int j=0;j<n;j++){
                    C[i][j] = new JTextField();
                    C[i][j].setBounds(x + j*50, y + i*40, 40, 30);
                    C[i][j].setEditable(false);
                    f.add(C[i][j]);
                }
            }

            JButton add = new JButton("Add");
            add.setBounds(250, y + n*50, 80, 30);
            f.add(add);

            add.addActionListener(ev -> {
                for(int i=0;i<n;i++){
                    for(int j=0;j<n;j++){
                        int a = Integer.parseInt(A[i][j].getText());
                        int b = Integer.parseInt(B[i][j].getText());
                        C[i][j].setText(String.valueOf(a + b));
                    }
                }
            });

            f.repaint();
        });

        f.setSize(700, 500);
        f.setLayout(null);
        f.setVisible(true);
        f.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
    }
}
```
<img width="315" height="118" alt="image" src="https://github.com/user-attachments/assets/e35d4daa-b177-45eb-8d0d-18315d2de7cb" />
<img width="452" height="238" alt="image" src="https://github.com/user-attachments/assets/4cb09acd-3d2c-497d-94ee-58efdf86787b" />


## Assi-16
```
import javax.swing.*;
import java.awt.*;

class ShapesDemo {
    public static void main(String[] args){

        JFrame f = new JFrame("Shapes");
        f.setSize(700,700);
        f.setLayout(null);

        JButton b1 = new JButton("Circle");
        JButton b2 = new JButton("Rectangle");
        JButton b3 = new JButton("Square");
        JButton b4 = new JButton("Line");
        JButton b5 = new JButton("Fill Circle");

        b1.setBounds(30,20,120,60);
        b2.setBounds(30,100,120,60);
        b3.setBounds(30,180,120,60);    
        b4.setBounds(30,260,120,60);
        b5.setBounds(30,340,120,60);

        f.add(b1);
        f.add(b2);  
        f.add(b3);
        f.add(b4);
        f.add(b5);

        String[] shape = {""};
        

        JPanel panel = new JPanel(){
            protected void paintComponent(Graphics g){
                super.paintComponent(g);

                if(shape[0].equals("Circle"))
                    g.drawOval(100, 150, 100, 100);
                else if(shape[0].equals("Rectangle"))
                    g.drawRect(100,150,100,60);
                else if(shape[0].equals("Square"))
                    g.drawRect(100,150,50,50);
                else if(shape[0].equals("Line"))
                    g.drawLine(100,150,100,100);
                else if(shape[0].equals("Fill Circle"))
                    g.fillOval(100,150,100,100);
            }
        };

        panel.setBounds(150, 50, 220, 250);
        f.add(panel);

        b1.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent e) {
                shape[0] = "Circle";
                panel.repaint();
         }
        });
        b2.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent e) {
                shape[0] = "Rectangle";
                panel.repaint();
         }
        });
        b3.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent e) {
                shape[0] = "Square";
                panel.repaint();
         }
        });
        b4.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent e) {
                shape[0] = "Line";
                panel.repaint();
         }
        });
        b5.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent e) {
                shape[0] = "Fill Circle";
                panel.repaint();
         }
        });

        f.setVisible(true);
        f.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);

    }
}
```
<img width="353" height="200" alt="image" src="https://github.com/user-attachments/assets/de942b41-22f2-4fe3-a9a8-ed8a66fc7b10" />
<img width="354" height="196" alt="image" src="https://github.com/user-attachments/assets/08e49859-cb46-4cc4-9687-37936bd5890e" />



## Assi-17
```
import javax.swing.*;
import java.awt.*;
import java.awt.event.*;

public class PaintBrush extends JFrame {

    int x, y;
    Color color = Color.BLACK;
    int size = 5;

    public PaintBrush() {
        setTitle("Paint Brush");
        setSize(600, 500);
        setLayout(new FlowLayout());

        JButton red = new JButton("Red");
        JButton green = new JButton("Green");
        JButton blue = new JButton("Blue");

        String sizes[] = {"5", "10", "15", "20"};
        JComboBox<String> cb = new JComboBox<>(sizes);

        add(red); add(green); add(blue); add(new JLabel("Size")); add(cb);

        red.addActionListener(e -> color = Color.RED);
        green.addActionListener(e -> color = Color.GREEN);
        blue.addActionListener(e -> color = Color.BLUE);

        cb.addActionListener(e -> {
            size = Integer.parseInt((String)cb.getSelectedItem());
        });

        addMouseMotionListener(new MouseMotionAdapter() {
            public void mouseDragged(MouseEvent e) {
                Graphics g = getGraphics();
                g.setColor(color);
                g.fillOval(e.getX(), e.getY(), size, size);
            }
        });

        setVisible(true);
        setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
    }

    public static void main(String[] args) {
        new PaintBrush();
    }
}
```
<img width="439" height="368" alt="image" src="https://github.com/user-attachments/assets/efa08a36-3223-4540-810d-e809993131eb" />



## Assi-18
```
package mypack;

public class A {
    public void showA() {
        System.out.println("Class A method");
    }
}
```
```
package mypack;

public class B {
    public void showB() {
        System.out.println("Class B method");
    }
}
```
```
package mypack;

public class C {
    public void showC() {
        System.out.println("Class C method");
    }
}
```
```
package mypack;

public class D {
    public void showD() {
        System.out.println("Class D method");
    }
}
```
```
package mypack;

public class E {
    public void showE() {
        System.out.println("Class E method");
    }
}
```
```
import mypack.*;

public class TestPackage {
    public static void main(String[] args) {

        A a = new A();
        B b = new B();
        C c = new C();
        D d = new D();
        E e = new E();

        a.showA();
        b.showB();
        c.showC();
        d.showD();
        e.showE();
    }
}
```
<img width="367" height="245" alt="image" src="https://github.com/user-attachments/assets/450120f8-c0c4-4da1-8c74-40137b2210a9" />


## Assi-19
```
package mypack;

public class A {
    public void showA() {
        System.out.println("Class A in mypack");
    }
}
```
```
package mypack.subpack;

public class B {
    public void showB() {
        System.out.println("Class B in subpackage");
    }
}
```
```
import mypack.A;
import mypack.subpack.B;

public class Test {
    public static void main(String[] args) {

        A a = new A();
        B b = new B();

        a.showA();
        b.showB();
    }
}
```
<img width="370" height="186" alt="image" src="https://github.com/user-attachments/assets/66e9a62c-98c4-4ba2-a547-816fd68457fc" />


## Assi-20
```
public class ExceptionDemo {
    public static void main(String[] args) {

        try {
            int arr[] = new int[5];

            arr[0] = 10;
            arr[1] = 20;
            arr[2] = 30;
            arr[3] = 40;
            arr[4] = 50;
            arr[5] = 60;

        } catch (ArrayIndexOutOfBoundsException e) {
            System.out.println("Error: Array index is out of bounds!");
        }

        try {
            int a = 10;
            int b = 0;

            int result = a / b; 

        } catch (ArithmeticException e) {
            System.out.println("Error: Cannot divide by zero!");
        }

        System.out.println("Program continues after handling exceptions...");
    }
}
```
<img width="443" height="215" alt="image" src="https://github.com/user-attachments/assets/c7cce9b1-ab36-4666-8297-db665552f8b6" />


## Assi-21
```
class InvalidAgeException extends Exception {
    InvalidAgeException(String msg) {
        super(msg);
    }
}

public class AgeTest {

    static void checkAge(int age) throws InvalidAgeException {
        if (age < 18 || age > 25) {
            throw new InvalidAgeException("Age must be between 18 and 25!");
        } else {
            System.out.println("Valid age. Student allowed.");
        }
    }

    public static void main(String[] args) {

        int age = 16; // change value to test

        try {
            checkAge(age);
        } catch (InvalidAgeException e) {
            System.out.println("Exception: " + e.getMessage());
        }
    }
}
```
<img width="399" height="166" alt="image" src="https://github.com/user-attachments/assets/61eb4d90-d47d-4499-b55d-ba8dfbc7f7c6" />


## Assi-22
```
import java.io.*;

public class CharFileCopy {
    public static void main(String[] args) {
        try {
            FileReader fr = new FileReader("source.txt");
            FileWriter fw = new FileWriter("dest_char.txt");

            int ch;

            while ((ch = fr.read()) != -1) {
                fw.write(ch);
            }

            fr.close();
            fw.close();

            System.out.println("File copied using character stream");
        } catch (Exception e) {
            System.out.println(e);
        }
    }
}
```

```
import java.io.*;

public class ByteFileCopy {
    public static void main(String[] args) {
        try {
            FileInputStream fis = new FileInputStream("source.txt");
            FileOutputStream fos = new FileOutputStream("dest_byte.txt");

            int b;

            while ((b = fis.read()) != -1) {
                fos.write(b);
            }

            fis.close();
            fos.close();

            System.out.println("File copied using byte stream");
        } catch (Exception e) {
            System.out.println(e);
        }
    }
}
```

## Assi-23
```
import java.util.*;
public class ArrayListDemo {
    public static void main(String[] args){
        ArrayList<String>list = new ArrayList<>();
        list.add("Apple");
        list.add("Banana");
        list.add("Mango");
        
        list.add(1,"Orange");
        
        System.out.println("Element at index 2: "+ list.get(2));
        
        list.set(0,"Grapes");
        list.remove("Banana");
        
        System.out.println("Size: "+ list.size());
        
        System.out.println("Contains Mangoes?"+ list.contains("Mango"));
        
        System.out.println("List Elements:");
        for(String item: list){
            System.out.println(item);
        }        
        
        list.clear();
        System.out.println("Is empty?"+ list.isEmpty());
    }
}
```
<img width="366" height="313" alt="image" src="https://github.com/user-attachments/assets/e0d519f5-9da3-4214-bfb6-8058e519fcc9" />

```
import java.util.*;
public class LinkedListExample {
    public static void main(String[] args){
        LinkedList<String> list = new LinkedList<>();
        
        list.add("Apple");
        list.addFirst("Banana");
        list.addLast("Mango");
        
        System.out.println("First: "+ list.getFirst());
        System.out.println("Last: "+ list.getLast());
        
        list.set(1,"orange");
        list.removeFirst();
        list.removeLast();
        
        System.out.println("Size: "+ list.size());
        
        System.out.println("List Elements:");
        for(String item: list){
            System.out.println(item);
        } 
        
        System.out.println("Contains Orange?"+ list.contains("Orange")); 
        
        list.clear();
        System.out.println("Is empty?"+ list.isEmpty());
        
    }
}
```
<img width="374" height="280" alt="image" src="https://github.com/user-attachments/assets/c2170e24-7a3d-4627-93c0-cc43a70a7072" />


```
import java.util.Stack;

public class Main {
    public static void main(String[] args) {
        Stack<Integer> stack = new Stack<>();

        // Push elements
        stack.push(10);
        stack.push(20);
        stack.push(30);

        System.out.println("Stack: " + stack);

        // Peek top element
        System.out.println("Top element: " + stack.peek());

        // Pop element
        System.out.println("Removed: " + stack.pop());

        System.out.println("Stack after pop: " + stack);
    }
}
```
<img width="368" height="223" alt="image" src="https://github.com/user-attachments/assets/544dc195-2fa6-4e49-87f4-1d340cf2cee4" />


```
import java.util.HashMap;

public class Main1 {
    public static void main(String[] args) {
        HashMap<Integer, String> map = new HashMap<>();

        map.put(1, "Apple");
        map.put(2, "Banana");
        map.put(3, "Mango");

        System.out.println(map.get(2)); // Banana

        map.remove(1);

        System.out.println(map.containsKey(3)); // true
    }
}
```
<img width="370" height="183" alt="image" src="https://github.com/user-attachments/assets/7f5544c8-22f1-4662-af70-e83b565f1e8e" />


```
import java.util.Hashtable;

public class Main1 {
    public static void main(String[] args) {

        Hashtable<Integer, String> ht = new Hashtable<>();

        ht.put(10, "A");
        ht.put(20, "B");

        System.out.println(ht.get(10));
    }
}
```
<img width="376" height="170" alt="image" src="https://github.com/user-attachments/assets/9ba4f84f-fbc2-45ed-9020-b4ffdc7624c9" />

