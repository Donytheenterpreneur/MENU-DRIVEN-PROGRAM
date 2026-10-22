//# MENU-DRIVEN-PROGRAM
//this is the basic menu driven program using switch in c
#include<stdio.h>
int main()
{
    int choice;
    float a,b;
    printf("MENU DRIVEN CALCULATOR\n");
    printf("1.addition\n");
    printf("2.subraction\n");
    printf("3.multiplication\n");
    printf("4.division\n");
    printf("enter your choice: ");
    scanf("%d",&choice);
    printf("enter your numbers: ");
    scanf("%f %f",&a,&b);
    switch(choice)
    {
        case 1: 
        printf("sum= %.2f",a+b);
        break;
        case 2:
        printf("difference=%.2f",a-b);
        break;
        case 3:
        printf("product=%.2f",a*b);
        break;
        case 4:
        if(b!=0)
        {
            printf("quotient=%.2f",a/b);
        }
        else
        {
            printf("division by zero is not allowed");
        }
        break;
        default:
        printf("invalid choice");

    }
    return 0;

}
