[Program-1 Program to add two distances](#Assi-1)
[Program-2 Program to print multiples of input values](#Assi-2)

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
