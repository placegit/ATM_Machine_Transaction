#include<stdio.h>
#include<stdlib.h>
int main()
{
	int balance=10000,tamt=0,choice=0;
	system("clear");
	printf("Varsha Singh Parihar\n");
	printf("---------------------\n");
	printf("ATM Cash Withdrawal\n\n");
	printf("1: Withdraw | 2. Exit\n");
	printf("Enter your choice:");
	scanf("%d",&choice);
	switch(choice)
	{
		case 1:
			printf("Your current balance:%d\n", balance);
			printf("\nEnter withdrawal amt:");
			scanf("%d",&tamt);
			if (tamt<=balance)
			{
				balance=balance-tamt;
				printf("Success...Collect your cash ");
				printf("\nYour Updated balance:%d",balance);
			}
			else
			{
				printf("Transaction Decline...Insuffient funds");
				
			}
			break;
			case 2:
				printf("\nThank you...visit again!");
				break;
			default:
				printf("\nInvalid input..try again!");
				break;
			}					
	
	
	printf("\n\n");
	return 0;
}
