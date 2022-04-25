/*
* Name: Test.c
* Program to create a slot machine
* Start Date: 3/27/2022
* Author: Lexis Bala
*/



#include<stdio.h>
#include<conio.h>

void main()
{
	int a = 0, b = 0, c = 0;
	clrscr();
	printf("\n\t\t press any key to play...\n");
	getch();
	for( ;kbhit(); )
	{
		delay(80);
		a++;
		b++;
		c++;
		gotoxy(20, 10);
		printf("%d %d %d", (a - 1), (b - 1), (c - 1));
		if (a == 10)
		{
			a = 0;
		}
		if (b == 10)
		{
			b = 4;
		}
		if (c = 10)
		{
			c = 0;
		}
	}
getch();
printf("\n\t\t");
if (a == b && b == c)
{
	printf("n\n***-: you win the game :-***")
}
else
{
	printf("\n ***-: you lose the game :-***\n-> try again");
}
}
