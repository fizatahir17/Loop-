# Loop-
Loop Constructs

Loop:
         A statement or set of statement that is executed repeatedly is known as loop.The structure that repeat a statements is known as iterative,repetitive or looping construct.

Loop are basically two purpose:
They are used to execute a statement or number of statements for a specified number of times.
For Example:a loop can be used to display a message on screen for 10 times.
They are used to get a sequence of values.
For Example::a loop can be used to display a sequence of numbers form 1 to 10.
Types of Loop:
1.for loop.
2.while loop.
3.do while loop.

1.for loop:
for loop executes one or more statements for a specified number of times.This loop is also called counter-controlled loop.It is the most flexible loop.That is why the most programmers use this loop in programs.
Syntax:
for(initilization;condition;increment/decrement)
Initialization:
                      It specifies the starting value of counter variables.One or many variables can be initialized in this part.To initialize many variables,each variable is separated by comma.
Condition:
                 The condition is given as a relational expression.The statement is executed only if the given condition is true. If the condition is false,the statement is never executed.
Statement:
                Statement is the instruction that is executed when the condition is true. If two or more statements are used,these are given in braces{}.It is called the body of the loop. 
Working “for” Loop:
The number of iterations depends on the initialization,condition and increment/decrement parts.The initialization part is executed only once when the control enters the loop.After initialization,the given condition is evaluated.If it is true,the control enters the body of loop and executes all statements in it.Then the increment / decrement part is executed that changes the value of counter variable.
Why it is called for loop?
Its called for loop because it repeats an action for a specific numbers of times or for each time in a sequence.
Do this for each number.
Do this for each items.
Do this for 10 times.

Examples: 
#include<iostream>
using namespace std;
int main()
{
	for(int a=1;a<=10;a++)
	{
		cout<<"hello";
	}
	return 0;
}
Output:hellohellohellohellohellohellohellohellohellohello

Program: 
#include<iostream>
using namespace std;
int main()
{
	for(int a=4;a<10;a++)
	{
		cout<<"fiza";
	}
	return 0;
}
Output: fizafizafizafizafizafiza

Program:
#include<iostream>
using namespace std;
int main()
{
	for(int a=4;a>10;a++)
	{
		cout<<"hello";
	}
	{
	cout<<"word";
}
return 0;
}
Output: word

Program:
#include<iostream>
using namespace std;
int main()
{
	for(int a=4;a<=10;a++)
	{
	a=57;
	cout<<a;
	cout<<"hello";
	}
return 0;
}
Output: 57hello

Program:
#include<iostream>
using namespace std;
int main()
{
	for(int a=4;a<=10;a++)
	{
	cin>>a;
	cout<<a;
	cout<<"hello";
	}
return 0;
}
Output: 11
11hello

Program:
#include<iostream>
using namespace std;
int main()
{
	for(int a=4;a<=10;a++)
	{
	}
	cout<<a;
	cout<<"hello";
return 0;
}
Output: 15hello

Program:
#include<iostream>
using namespace std;
int main()
{
	for(int a;a<=10;a++)
	{
	cout<<a;
}
return 0;
}
Error:
int a;declare a but does not initialize it.
In C++, an uninitialized local variable contains garbage value.
So a could start at any number, not a necessarily 0 or 1.
If garbage value is greater than 10 the loop may never run.
If garbage value is small,the loop may print strange number untill a exceeds 10.

Correct:
#include<iostream>
using namespace std;
int main()
{
	for(int a=1;a<=10;a++)
	{
	cout<<a;
}
return 0;
}
Output: 12345678910

Program:
#include<iostream>
using namespace std;
int main()
{
	for(int a=1;a<=10;)
	{
	cout<<a;
}
return 0;
}
Output: 111111111infinite loop

Program:
#include<iostream>
using namespace std;
int main()
{
	for(int a=1;a<=10;)
	{
	cout<<a;
	a=a+3;
}
return 0;
}
Output: 14710

Program:
#include<iostream>
using namespace std;
int main()
{
	for(int a=1;a<=10;a++)
	{
	cout<<a;
	a=a+3;
}
return 0;
}
Output: 159

Program:
#include<iostream>
using namespace std;
int main()
{
	for(int a=1;a<=10;a++);
	{
	cout<<a;
	a=a+3;
}
return 0;
}
Error:
The semicolon end the loop immediately, so the loop run but does nothing.
Then the block below becomes an independent block,not a part of loop.
Output: 11

Program:
#include<iostream>
using namespace std;
int main()
{
	int a=1;
	for(a=3;a<=10;a++);
	{
	cout<<a;
	a=a+3;
}
return 0;
}
Output: 11

Program:
#include<iostream>
using namespace std;
int main()
{
	int a=1;
	for( ;a<=10;a++);
	{
	cout<<a;
	a=a+3;
}
return 0;
}
Output: 11

Program:
#include<iostream>
using namespace std;
int main()
{
	int a=1;
	for(a=3 ; ;a++);
	{
	cout<<a;
	a=a+3;
}
return 0;
}
Output: 37infinite loop

Program:
#include<iostream>
using namespace std;
int main()
{
	int a=3;
	for( ;a<=10;a++);
	{
	cout<<a;
	a=a+5;
}
return 0;
}
Output: 39

Program:
#include<iostream>
using namespace std;
int main()
{
int a=3;
	for(a=2 ;a<=10; )
	{
	cout<<a;
}
return 0;
}
Output: 222222222222infinite loop

Program:
3,6,9,12,……………………………….,99

#include<iostream>
using namespace std;
int main()
{
int a=3;
	for(a=3;a<=99;a++)
	{
	cout<<a;
	a=a+3;
}
return 0;
}
Output: 371115192327313539434751555963677175798387919599

Program:
1+2+3+4+5

#include<iostream>
using namespace std;
int main()
{
int a,sum=0;
	for(a=1;a<=5;a++)
	{
sum=sum+a;
}
cout<<"sum=";
cout<<sum;
return 0;
}
Output: sum=15 

Program:
100,98,96,94,…………………………………………..52

#include<iostream>
using namespace std;
int main()
{
	for(int a=100;a<=52;a++)
	{
cout<<a;
}
return 0;
}

Program:
1*2*3*4
#include<iostream>
using namespace std;
int main()
{
	int multiply=1;
	for(int a=1;a<=5;a++)
	{
multiply=multiply*a;
}
cout<<"multiply=";
cout<<multiply;
return 0;
}
Output: multiply=120

Program:
#include<iostream>
using namespace std;
int main()
{
	float factorial;
	int n;
cout<<"enter positive integer";
cin>>n;
for(int a=1;a<=n;a++)
{
	factorial=factorial*a;
	cout<<"factorial=";
	cout<<factorial;
}
return 0;
}
Output: enter positive integer4
factorial=0factorial=0factorial=0factorial=0

Program:
#include<iostream>
using namespace std;
int main()
{
for(int a=2;a<=10;a++)
{
cout<<a;
a=a+4;
}
return 0;
}
Output:  27

Program:
2*1=2
2*2=4
….…….
….…….
2*10=20

#include<iostream>
using namespace std;
int main()
{
int n;
cout<<"enter a number=";
cin>>n;
cout<<"\n multiplication table of";
cout<<n;
cout<<"\n";
for(int i=1;i<=10;i++)
{
	cout<<n;
	cout<<"*";
	cout<<i;
	cout<<"=";
	cout<<n*i;
	cout<<"\n";
}
return 0;
}
Output: enter a number=2

 multiplication table of2
2*1=2
2*2=4
2*3=6
2*4=8
2*5=10
2*6=12
2*7=14
2*8=16
2*9=18
2*10=20

while-loop:
                  while loop is the simplest loop of C language. This loop executes one or more statements while the given condition remains true.It is useful where the number of iterations not known in advance.

Syntax: 
while(condition) 

Condition:
                 The condition is given as relational expression.It controls the iteration of loop.The statement is executed only if the given condition is true.If the condition is false,the statement is never executed.
Statement:
                 Statement is the instruction that is executed when the condition is true. Two or more statements are specified in braces {}.It is called the body of the loop.

Working of “while” loop:
                                          The condition is evaluated first.If it is true,the control enters the body of the loop and executes all statements in the body.The control moves to the start of the loop and evaluated the condition again.This process continues as long as the condition remains true.The loop is terminated when conditions becomes false.The loop never ends if the condition remains true.A loop never ends is known as an infinite loop.
Example:
#include<iostream>
using namespace std;
int main()
{
int n=1;
while(n<=5)
{
	cout<<"hello";
	n++;
}
return 0;
}
Output:  hellohellohellohellohello

Program:
#include<iostream>
using namespace std;
int main()
{
int n=1;
while(n<=10)
{
	cout<<"hello";
	n=n+4;
}
return 0;
}
Output: hellohellohello

Program:
#include<iostream>
using namespace std;
int main()
{
int n=5,sum=0;
while(n<=10)
{
	cout<<"ayesha";
	n=n+4;
	sum=sum+n;
}
cout<<"\nsum=";
cout<<sum;
return 0;
}
Output: ayeshaayesha
sum=22

do-while loop:
                      The do while loop is an iterative control in C language.This loop executes one or more statements while the condition is true.The condition in this loop checked after the body of loop.That is why it is executed at least once.

Syntax:
do
{
Statements;
}
while(condition);

do: 
It is the keyword that indicate the start of the loop.
Condition:
                 The condition is given as relational expression.It controls the iteration of loop.The statement is executed only if the given condition is true.If the condition is false,the statement is never executed.
Statement:
                 Statement is the instruction that is executed when the condition is true. Two or more statements are specified in braces {}.It is called the body of the loop.



Important point:
                The important point about do-while loop is that the condition ends with semi-colon.An error occurs if the semicolon is not used at the end of the condition.

Working of “do while” loop:
                           The body of loop is executed first.The condition is check after executing the statements in loop body.The control again enters the body of the loop and executes all statements in the body if the condition is true,This process continues as long as the condition remains true.The loop terminates when the condition becomes false.The loop executes at least once even if the condition is false in the start.
Example:
#include<iostream>
using namespace std;
int main()
{
int a=1;
do
{
	cout<<"hello";
	a++;
}
while(a<=5);
return 0;
}
Output: hellohellohellohellohello

Program:
#include<iostream>
using namespace std;
int main()
{
	cout<<"\noutput of for loop is:\n";
int a=3;
for(a=3;a<=99; )
{
	cout<<a;
	cout<<" ";
	a=a+3;
}
cout<<"\noutput of while loop is:\n";
int b=3;
while(b<=99)
{
	cout<<b;
	cout<<" ";
	b=b+3;
}
cout<<"\noutput of do while loop is:\n";
int c=3;
do
{
	cout<<" ";
	cout<<c;
	c=c+3;
}
while(c<=99);
return 0;
}
Output:
output of for loop is:
3 6 9 12 15 18 21 24 27 30 33 36 39 42 45 48 51 54 57 60 63 66 69 72 75 78 81 84 87 90 93 96 99
output of while loop is:
3 6 9 12 15 18 21 24 27 30 33 36 39 42 45 48 51 54 57 60 63 66 69 72 75 78 81 84 87 90 93 96 99
output of do while loop is:
 3 6 9 12 15 18 21 24 27 30 33 36 39 42 45 48 51 54 57 60 63 66 69 72 75 78 81 84 87 90 93 96 99

Nested loop:

A loop within loop called nested loop.In nested loop,the inner loop is executed completely with each change in the value of counter variable of outer loop.
The nesting loop can be done up to level.the increase in level of nesting increases the complexity of nested loop.Any loop can be used as inner loop of another loop.
Syntax:

for(initialization;condition;increment/decrement)
{
for(initialization;condition;increment/decrement)
{
Statements;
}
}

Program
#include<iostream>
using namespace std;
int main()
{
	for(int i=1;i<=3;i++)
	{
		for(int j=1;j<=2;j++)
		{
			cout<<"hello";
			cout<<"   ";
		}
		cout<<"\n";
	}
}

Output:  hello   hello
hello   hello
hello   hello

Program:
#include<iostream>
using namespace std;
int main()
{
	for(int i=1;i<=3;i++)
	{
		for(int j=1;j<=2;j++)
		{
			cout<<"i=";
			cout<<i;
			cout<<"  ";
			cout<<"j=";
			cout<<j;
			cout<<"  ";
		}
		cout<<"\n";
	}
}

Output:
i=1  j=1i=1  j=2
i=2  j=1i=2  j=2
i=3  j=1i=3  j=2

Program:
#include<iostream>
using namespace std;
int main()
{
	for(int i=1;i<=4;i++)
	{
		for(int j=1;j<=i;j++)
		{
			cout<<"?";
		}
		cout<<"\n";
	}
}
Output: 
?
??
???
????

Program:
#include<iostream>
using namespace std;
int main()
{
	for(int i=1;i<=4;i++)
	{
		for(int j=1;j<=i;j++)
		{
			cout<<"  ";
		}
		cout<<"*";
		cout<<"\n";
	}
}

Output: 
 *
    *
      *
        *


Program:
#include <iostream>
using namespace std;

int main() {
    int n = 10; 
    for (int i = 1; i <= n; i++) {
        for (int j = 1; j <= i; j++) {
            cout << "*";
        }
        cout << "\n"; 
    }
    return 0;
}

Output:
*
**
***
****
*****
******
*******
********
*********
**********

Program:
#include <iostream>
using namespace std;
int main() {
    int n = 10;  
    for (int i = 0; i < n; i++) {
        for (int s = 0; s < i + 2; s++)
            cout << " ";
        for (int j = 0; j < n - i; j++)
            cout << "*";
        cout <<"\n";
    }
    return 0;                                               
}  
                                       
Output:
  **********
   *********
    ********
     *******
      ******
       *****
        ****
         ***
          **
           *

Program:
#include <iostream>
using namespace std;
int main() {
    int n = 5;
    for (int i = 1; i <= n; i++) {
        for (int s = 1; s <= n - i; s++)
            cout << " ";
        for (int j = 1; j <= 2*i - 1; j++)
            cout << "*";
        cout << "\n";
    }
    return 0;
}
Output:
 *
   **
  ***
 ****
*****

Program:
#include <iostream>
using namespace std;
int main() {
    int n = 5;
    for (int i = 1; i <= n; i++) {
        for (int s = 1; s <= n - i; s++)
            cout << " ";
        for (int j = 1; j <= 2 * i - 1; j++)
            cout << "*";
        cout << endl;
    }
    for (int i = n - 1; i >= 1; i--) {
        for (int s = 1; s <= n - i; s++)
            cout << " ";
        for (int j = 1; j <= 2 * i - 1; j++)
            cout << "*";
        cout << endl;
    }
    return 0;
}

Output:
      
    *
   ***                                                                
  *****
 *******
*********
 *******
  *****
   ***
    *

Array:
An array is a collection of items stored at continuous memory locations, and all the items in an array are of the same data type.
Each item in an array is called an element, and every element is accessed using an index number.

Example:
int marks[5] = {90, 85, 88, 92, 80};

Program:
#include <iostream>
using namespace std;
int main() {
    int a[5];
    a[0]=3;
    a[1]=6;
    a[2]=9;
    a[3]=7;
    a[4]=2;
    cout<<a[0];
    cout<<a[1];
    cout<<a[2];
    cout<<a[3];
    cout<<a[4];
    return 0;
}

Output:  36972

Program:
#include <iostream>
using namespace std;
int main() {
    string name[5];
    name[0]="ayesha";
    name[1]="laiba";
    name[2]="hamna";
    name[3]="yashfa";
    name[4]="aimen";
    cout<<name[0];
    cout<<name[1];
    cout<<name[2];
    cout<<name[3];
    cout<<name[4];
    return 0;
}

Output:  ayeshalaibahamnayashfaaimen

Program:
#include <iostream>
using namespace std;
int main() {
    int b[7]={3,7,8,9,11,15,20};
    cout<<b[0];
    cout<<b[1];
    cout<<b[2];
    cout<<b[3];
    cout<<b[4];
    cout<<b[5];
    cout<<b[6];
    return 0;
}

Output:  3789111520

Program:
#include <iostream>
using namespace std;
int main() {
    float b[4]={2,4,6,8};
    cout<<b[0];
    cout<<b[1];
    cout<<b[2];
    cout<<b[3];
    return 0;
}

Output:    2468


Program:
#include <iostream>
using namespace std;
int main() {
	float sum;
    float b[4]={4,8,12,2};
    cout<<b[0];
    cout<<b[1];
    cout<<b[2];
    cout<<b[3];
    sum=b[0]+b[1]+b[2]+b[3];
    cout<<"sum=";
    cout<<sum;
    return 0;
}

Output:   48122sum=26

Program:
#include <iostream>
using namespace std;
int main() {
	int a[3][2],sum;
   cin>>a[0][0];
   cin>>a[0][1];
   cin>>a[1][0];
   cin>>a[1][1];
   cin>>a[2][0];
cin>>a[2][1];
sum=a[0][0]+a[0][1];
cout<<"\nsum=";
   cout<<sum;
   sum=a[1][0]+a[1][1];
   cout<<"\nsum=";
   cout<<sum;
   sum=a[2][0]+a[2][1];
    cout<<"\nsum=";
    cout<<sum;
    return 0;
}

Output:
2
3
7
5
9
10

sum=5
sum=12
sum=19

Program:
#include <iostream>
using namespace std;
int main() {
	int a[2][3];
	cin>>a[0][0]>>a[0][1]>>a[0][2];
  cin>>a[1][0]>>a[1][1]>>a[1][2];
  for(int b=0;b<=1;b++)
  {
  	for(int c=0;c<=2;c++)
{
	cout<<a[b][c];
}
  }
    return 0;
}

Output:   
2
25
77
58
34
99
22577583499

Program:
Addition of Two Matrices using 2D Arrays
#include <iostream>
using namespace std;
int main() {
    int rows = 2, cols = 2;
    int matrix1[2][2] = {{1, 2}, {3, 4}};
    int matrix2[2][2] = {{5, 6},{7, 8}};
    int sum[2][2];
    for (int i = 0; i < rows; i++) {
        for (int j = 0; j < cols; j++) {
            sum[i][j] = matrix1[i][j] + matrix2[i][j];
        }
    }
    cout << "Sum of the matrices:\n";
    for (int i = 0; i < rows; i++) {
        for (int j = 0; j < cols; j++) {
            cout << sum[i][j] << " ";
        }
        cout << endl;
    }
    return 0;
}
Output:Sum of the matrices:

6 8
10 12

Program 
Sum of each row
#include <iostream>
using namespace std;
int main() {
    int rows, cols;
   int a[4][3]={{4,4,4},{8,8,8},{6,6,6},{10,10,10}};
   int sum=0;
   for(int r=0;r<=3;r++)
   {
   	for(int c=0;c<=2;c++)
   	{
   		sum=sum+a[r][c];
	   }
   }
   cout<<"sum="<<sum;
}
Output:
sum=84

Program:
sum of each column

#include <iostream>
using namespace std;
int main()
{
    int a[3][3], colSum;
    for(int i = 0; i < 3; i++)
    {
        for(int j = 0; j < 3; j++)
        {
            cin >> a[i][j];
        }
    }
    for(int j = 0; j < 3; j++)
    {
        colSum = 0;
        for(int i = 0; i < 3; i++)
        {
            colSum += a[i][j];
        }
        cout << "Sum of column " << j+1 << " = " << colSum << endl;
    }
}
Output:
1
2
3
4
5
6
7
8
9
Sum of column 1 = 12
Sum of column 2 = 15
Sum of column 3 = 18
Program
Sum of each row
#include <iostream>
using namespace std;
int main()
{
	int rows=3;
	int column=3;
    int arr[3][3]={{1,2,3},{4,5,6},{7,8,9}};
    for(int i = 0; i < 3; i++)
    {
    		int sum=0;
        for(int j = 0; j < 3; j++)
        {
         sum=sum+ arr[i][j];   
        }
        cout << "Sum of row no" << i+1<<"is"<<sum << endl;
    }
}
Output:

Sum of row no1is6
Sum of row no2is15
Sum of row no3is24  

Program
#include <iostream>
using namespace std;
int main() {
    int arr[3][3] = {{1, 2, 3}, {4, 5, 6}, {7, 8, 9}};
    int totalSum = 0;
    for (int i = 0; i < 3; i++) {
        for (int j = 0; j < 3; j++) {
            totalSum += arr[i][j];
        }
    }
    cout << "Sum of all elements in the 2D array = " << totalSum << endl;
    return 0;
}
Output:
Sum of all elements in the 2D array = 45

Program
Multiple each element of 2D with no.5
#include <iostream>
using namespace std;

int main() {
    int arr[2][3] = {{1, 2, 3},{4, 5, 6}};
    for (int i = 0; i < 2; i++) {
        for (int j = 0; j < 3; j++) {
            arr[i][j] = arr[i][j] * 5;
        }
    }
    cout << "Array after multiplying each element by 5:\n";
    for (int i = 0; i < 2; i++) {
        for (int j = 0; j < 3; j++) {
            cout << arr[i][j] << " ";
        }
        cout << endl;
    }
    return 0;
}
Output:
Array after multiplying each element by 5:
5 10 15
20 25 30

Program :
#include <iostream>
using namespace std;
int main()
{
    int a[10] = {1, 2, 3, 4, 5, 6};
    int n = 6;                   
    int even = 0, odd = 0;
    cout << "Even numbers: ";
    for (int i = 0; i < n; i++)
    {
        if (a[i] % 2 == 0)
        {
            cout << a[i] << " ";
            even++;
        }
    }
    cout << "\nOdd numbers: ";
    for (int i = 0; i < n; i++)
    {
        if (a[i] % 2 != 0)
        {
            cout << a[i] << " ";
            odd++;
        }
    }
    cout << "\nTotal Even = " << even;
    cout << "\nTotal Odd = " << odd;
    return 0;
}
Output:
Even numbers: 2 4 6
Odd numbers: 1 3 5
Total Even = 3
Total Odd = 3

Program:
#include <iostream>
using namespace std;
int main()
{
    int a[10] = {1, 2, 3, 4, 5, 6, 7};
    int n = 7;
    int even = 0, odd = 0;
    for (int i = 0; i < n; i++)
    {
        if (a[i] % 2 == 0)
            even++;
        else
            odd++;
    }
    cout << "Even numbers = " << even << endl;
    cout << "Odd numbers = " << odd << endl;
    return 0;
}
Output:
Even numbers = 3
Odd numbers = 4

Program:
#include <iostream>
using namespace std;
int main()
{
    int a[3][3];
    int sum = 0;
    for(int i = 0; i < 3; i++)
    {
        for(int j = 0; j < 3; j++)
        {
            cin >> a[i][j];
        }
    }
    for(int i = 0; i < 3; i++)
    {
        for(int j = 0; j < 3; j++)
        {
            sum += a[i][j];
        }
    }
    cout << "Sum of all elements = " << sum;
}
Output:
4
5
6
7
8
9
2
3
4
Sum of all elements = 48

Structure:
           
Struct{

}stdstructname;

Program:
#include<iostream>
using namespace std;
int main()
{
	struct{
		int rollnumber;
		string subject[3];
		string name;
		int marks;
	}stdinfo;
	stdinfo.rollnumber=7;
	stdinfo.subject[0]="urdu";
	cin>>stdinfo.name;
	cout<<stdinfo.rollnumber;
}                         
Output:
  7
7

    
