Write a C program to record the marks of 20 students in a classroom.

#include<stdio.h>
#include<conio.h>

struct student
{
    int rollno,marks;
    char name[40];
};
int main()
{
    int i,n;
    struct student s[30];
    char sname[40];
    printf("ENTER THE NUMBER OF STUDENTS:");
    scanf("%d",&n);
    for(i=0;i<n;i++)
    {
        printf("\nENTER THE %d STUDENT DETAILS \n",i+1);
        printf("ENTER THE ROLLNO:\n");
        scanf("%d",&s[i].rollno);
        printf("\nENTER THE STUDENTS NAME:\n");
        scanf("%s",s[i].name);
        printf("\nENTER THE MARKS:\n");
        scanf("%d",&s[i].marks);
    }
    for(i=0;i<n;i++)
    {
        printf("\nSTUDENTS DETAILS ARE\n");
        printf("\nROLL NO\t\tNAME\t\tMARKS\n");
    }
    for(i=0;i<n;i++)
    {
        printf("%d\t\t%s\t\t%d\t\t\n",s[i].rollno,s[i].name,s[i].marks);
    }
       return 0;
       
    }
    

