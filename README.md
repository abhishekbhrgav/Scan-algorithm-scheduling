# Scan-algorithm-scheduling
Implement Scan algorithm for scheduling
#include<stdio.h>
#include<conio.h>
int main()
{
	int number,head,prevoius,current,i=0;
	int process[11];
	printf("enter the number of process");
	scanf("%d",&number);
	printf("enter which is currently running");
	scanf("%d",&current);
	printf("enter the processes which are remaining");
	for(i=0;i<number;i++)
	{
		scanf("%d",&process[i]);
	}
	printf("the sequence of entertaining the processes are:\n");
	for(i=0;i<number;i++)
	{
		printf("%d\n",process[i]);
	}
	}
