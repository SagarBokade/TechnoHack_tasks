#include<stdio.h>
#include<string.h>

struct employee
{
	char name[25];
	int empid;
	int age;
	char des[50];
	float gsal;
	float bsal;
};

int main()
{
	int i;
	struct employee e[2];
	for(i=0;i<=1;i++)
	{
		printf("Enter Name : \n");
		scanf("%s",e[i].name);
		printf("Enter employee id. : \n");
		scanf("%d",&e[i].empid);
		printf("Enter age : \n");
		scanf("%d",&e[i].age);
		printf("Enter designation: \n");
		scanf("%s",e[i].des);
		printf("Enter basic sal : \n");
		scanf("%f",&e[i].bsal);
		e[i].gsal=e[i].bsal+0.21*e[i].bsal+0.51*e[i].bsal+0.05*e[i].bsal;
		}
	for(i=0;i<=1;i++)
	{
		printf("Name : %s\n",e[i].name);
		printf("Employee id : %d\n",e[i].empid);
		printf("Age: %d\n",e[i].age);
		printf("Designation: %s\n",e[i].des);
		printf("Basic salaray: %d\n",e[i].bsal);
		printf("Gross salaray: %f\n",e[i].gsal);
		printf("\n\n\nThank you for using our services\n\n\n");
	}
	return 0;
}
