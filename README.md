#include<stdio.h>
#include<conio.h>
void main()
{
	int i,j,r,c,sum=0,a[3][3];
	printf("Enter the elements of the array\n");
	for(r=0;r<3;r++)
	{
		for(c=0;c<3;c++)
		{
			scanf("%d",&a[r][c]);
		}
	}
	printf("The entered array is \n");
	for(r=0;r<3;r++)
	{
		for(c=0;c<3;c++)
		{
            printf("%d\t",a[r][c]);
			if(r==c)
			{
				sum=sum+a[r][c];
			}
		}
		printf("\n");
	}
	printf("The sum of all the diagonal elements of the matrix is:- %d",sum);
	getch();
}
