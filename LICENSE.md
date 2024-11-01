#include <stdio.h>
#include <math.h>
int main()
{
	char a;
	printf("Please input a capital:\n");
	scanf("%c",&a);
	int h=(int)a-65+1;
	int y,q=h;
	for(int i=1;i<=h;i++)
	{
		y=65;
		for(int f=1;f<=q;f++)
		{
			printf(" ");
		}
		for(int n=1;n<=i;n++)
		{
			printf("%c",(char)y);
			y++;
		}
		   y=y-2;
		for(int m=1;m<=i-1;m++)
		{
			printf("%c",(char)y);
			y--;
		}
		printf("\n");
		q--;
	}
	return 0;
}
