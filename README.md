
#include<stdio.h>
#include<conio.h>
int main()
{
	int number,head,previous,current,i,t,j,n;
	int process[11];
	printf("----------WELCOME---------------\n");
	printf("enter the number of process");
	scanf("%d",&number);
	printf("\nenter which is currently running");
	scanf("%d",&current);
	printf("\nenter the process which is running previously");
	scanf("%d",&previous);
	printf("\nenter the processes which are remaining");
	for(i=0;i<number;i++)
	{
		scanf("%d",&process[i]);
	}
	
		for(i=0;i<(number-1);i++)
		{
			for(j=0;j<(number-i-1);j++)
			{
				if(process[j]>process[j+1])
				{
				t=process[j];
		 	    process[j]=process[j+1];
		 	    process[j+1]=t;
				}	
			}	
		}
		if(current>previous)
		{
			for(i=0;i<number;i++)
		{
			if(process[i]>current)
			{
				n=i;
				printf("\nThe sequence of entertaining proceses is :");
				for(n;n<number;n++)
				{
					printf("\n%d",process[n]);
				}
				n=i-1;
				for(n;n>=0;n--)
				{
					printf("\n%d",process[n]);
				}
				break;
			}
			else
			{
			}
		}
		}
		else
		{
			for(i=0;i<number;i++)
		{
			if(process[i]>current)
			{
				n=i-1;
				printf("\nThe sequence of entertaining proceses is :");
				for(n;n>=0;n--)
				{
					printf("\n%d",process[n]);
				}
				n=i;
				for(n;n<number;n++)
				{
					printf("\n%d",process[n]);
				}
				break;
			}
			else
			{
			}
		}
}
}
