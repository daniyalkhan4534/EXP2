# EXP2a

The programme is designed to calculate the average and sum of marks. The variable i is defined as integer. There is a for loop in use and variable i starts from 0 to 10 with an increment of 1. The marks are then scanned using the scanf function. Followed by the print statement "Enter marks for Student:" using the prinf function.

The aggregate, average and sum of the marks are now calculated using a another for loop. Sum is addition of all the marks. The average is the sum of all marks divided by the number of students. The total number of students in this case is 10, hence the sum of the marks is divided by  10.


The printf function is then used to output the following two print statements:

"Sum of the numbers" ; "Average of the numbers"

![image](https://user-images.githubusercontent.com/127819492/234346139-67eb9a98-b78f-49a1-83f1-c9e50fd5dcbb.png)

Code: #include <windows.h>
#include <stdio.h>


int main()
{
int marks[10],i,sum=0,avg;
for (i=0; i<10; i++)
{
    scanf("%d",&marks[i]);
    printf("\n Enter Marks for Student %d:", i+1);
}
for (i=0; i<10; i++)
{
    sum=marks[i]+sum;
    avg=sum/10;
}
printf("\n Sum of the numbers: %d",sum);
printf("\n Average of the numbers: %d",avg);
