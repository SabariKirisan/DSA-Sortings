## BASIC - 1 (JAVA)
## Problem-1:
Write a program that takes an integer, then a string, then a char from the user and prints them in the screen.

Input:  2 Name y

Expected Output:

2

Name

y

## PROGRAM:(Main.java)
```
import java.util.Scanner;
public class Main
{
    public static void main(String[] args)
    {
        int num;
        String name;
        char ch;
        Scanner input=new Scanner(System.in);
        num=input.nextInt();
        name=input.next();
        ch=input.next().charAt(0);
        System.out.println(num);
        System.out.println(name);
        System.out.println(ch);

    }
}
```

## OUTPUT
![image](https://github.com/user-attachments/assets/c9d58f12-d25a-4f6d-a62a-9ab1b785e555)

## Problem-2:
Write a program to check whether a triangle can be formed with the given values for the angles.

If sum of angles is equal to 180, then triangle can be formed, else it can't be formed.

Input: 45 45 45

Expected Output: 

Triangle cannot be formed

Explanation -> We are getting 3 inputs, that is three angles of triangle, but here the sum of three angles that is 45+45+45 is not equal to 180 so Triangle cannot be formed is the output.

## PROGRAM:(Main.java)
```
import java.util.*;
public class Main
{
    public static void main(String[] args)
    {
        Scanner input=new Scanner(System.in);
        int angle1=input.nextInt();
        int angle2=input.nextInt();
        int angle3=input.nextInt();
        if((angle1+angle2+angle3)==180)
        {
            System.out.println("Triangle can be formed");
        }
        else
        {
            System.out.println("Triangle cannot be formed");
        }
    }
}
```

## OUTPUT
![image](https://github.com/user-attachments/assets/576e853a-6966-4b60-b083-2af1113ee8d3)

## Problem-3:
Given mark of student, Print the Grade

Grade A if mark is greater than or equal to 90

Grade B if mark is greater than or equal to 80

Grade C if mark if greater than or equal to 60

Grade D if mark if greaer than or equal to 35

Fail if mark is lesser than 35


Input: 95

Expected Output:

Grade A

Explanation: Here 95 is greater than or equal to 90 so its Grade A

## PROGRAM:(Main.java)
```
import java.util.*;
public class Main
{
    public static void main(String[] args)
    {
        Scanner input=new Scanner(System.in);
        int mark=input.nextInt();
        if (mark>=90)
        {
            System.out.println("Grade A");
        }
        else if (mark>=80)
        {
            System.out.println("Grade B");
        }
        else if (mark>=60)
        {
            System.out.println("Grade C");
        }
        else if (mark>=35)
        {
            System.out.println("Grade D");
        }
        else
        {
            System.out.println("Fail");
        }
    }
}
```

## OUTPUT
![image](https://github.com/user-attachments/assets/1cd5671d-053b-4033-a3e2-414defcc1919)
![image](https://github.com/user-attachments/assets/8eae3224-d269-4031-9e66-e219ceed3cc9)
![image](https://github.com/user-attachments/assets/db200b33-1f87-4d27-8d92-afe48e42f44c)
![image](https://github.com/user-attachments/assets/5c3ff0b2-7210-4b34-94ec-29b3c71b2c3b)
![image](https://github.com/user-attachments/assets/c0f626bb-7566-4554-86c3-014f148ee249)


## Problem-4:
 Write a program using switch case which takes a value and prints the respective Size.
If size is 29 then its small

If size is 30 then its Medium

If size is 38 then its Large

If size is 42 then its XLarge

If size is not any of the above then Invalid.



Input: 29

Expected Output: 

Small
## PROGRAM:(Main.java) 
```
import java.util.*;
public class Main
{
    public static void main(String[] args)
    {
        Scanner input=new Scanner(System.in);
        int size=input.nextInt();
        switch (size)
        {
            case 29:
                System.out.println("Small");
                break;
            case 30:
                System.out.println("Medium");
                break;
            case 38:
                System.out.println("Large");
                break;
            case 42:
                System.out.println("XLarge");
                break;
            default:
                System.out.println("Invalid");
        }
        
    }
}
```
## OUTPUT
![image](https://github.com/user-attachments/assets/78410d7b-a425-4236-8a02-34911982b5dc)
![image](https://github.com/user-attachments/assets/e2b78a1e-1d91-4575-8f8b-e8b597273e1c)
![image](https://github.com/user-attachments/assets/3c90f133-636c-419d-bc86-0329941db656)
![image](https://github.com/user-attachments/assets/9dc2cecc-fdef-4127-9302-857a391ddeff)
![image](https://github.com/user-attachments/assets/f32a7856-822b-4cb5-a33c-bb00b8c11e2d)
