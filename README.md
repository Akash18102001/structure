#include<stdio.h>
#include<stdlib.h>

struct employee     //Defining structure employee
{
	char n[30];		//variable for emloyee's name
	int a;			//variable for emloyee's age
	char p[10];		//variable for emloyee's phone number 
	long int s;		//variable for emloyee's salary
};

main()
{
	int i;
	employee E[20];		//array to store structure values of all employees
	printf("-----------Enter the details of 20 employees.-----------\n\n");
	
	for(i=1;i<=20;i++) //Taking each employee detail as input
	{
		printf(" Employee Number : %d\n",i);
		printf(" Name : ");
		scanf("%s",&E[i].n);
		printf(" Age : ");
		scanf("%d",&E[i].a);
		printf(" Phone Number : ");
		scanf("%s",&E[i].p);
		printf(" Salary : ");
		scanf("%ld",&E[i].s);
		printf("\n");
	}
	printf("----------- Details of 20 Employees.-----------\n\n");
	for(i=1;i<=20;i++) //Displaying Employee details
	{
		printf(" Employee Number : %d \n",i);
		printf(" Name : %s \n",E[i].n);
		printf(" Age : %d \n",E[i].a);
		printf(" Phone Number : %s \n",E[i].p);
		printf(" Salary : %ld \n",E[i].s);
		printf("\n");
	}
	return 0;
}
