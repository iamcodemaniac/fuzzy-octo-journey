# fuzzy-octo-journey
/*一只公鸡值五钱，一只母鸡值三钱，三只小鸡值一钱，现在要用百钱买百鸡，请问公鸡、母鸡、小鸡各多少只？*/
#include <stdio.h>
int main()
{   int cock=0,hen=0,chicken=0;
	for(cock=0;cock<=20;cock++)
	{
		for(hen=0;hen<=33;hen++)
		{
			chicken=100-cock-hen;/*减少计算小鸡的循环*/ 
			if(cock*5+hen*3+chicken/3==100&&cock+hen+chicken==100)
			printf("公鸡有%d只,母鸡有%d只，小鸡有%d只\n",cock,hen,chicken);
		}
	}
	
}
