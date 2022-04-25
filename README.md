#include<stdio.h>
#include<math.h>
#define note
void addition();
void substraction();
void multiplicaliton();
void division();
void modulus();
void factorial();
void power();
void square();
void squareroot();
void cube();

int main(){
	printf("welcome to the scientific calculator\n");
	int choice;
	int i;
	printf("enter 1 for addition\n");
	printf("enter 2 for substraction\n");
	printf("enter 3 for multiplicaliton\n");
	printf("enter 4 for division\n");
	printf("enter 5 for modulus\n");
	printf("enter 6 for factorial\n");
	printf("enter 7 for power\n");
	printf("enter 8 for square\n");
	printf("enter 9 for squareroot\n");
	printf("enter 10 for cube\n");
	
	while(1){
		printf("\n\nenter the operation you want to do: \n");
		if(i = choice)
		{
		scanf("%d",& choice);
		}
		switch(choice){
			case 1:
				addition(); break;
			case 2:
			    substraction(); break;
				case 3:
				multiplicaliton();
				break;
				case 4:
				division(); break;
				case 5:
					modulus();
					break;
					case 6:
						factorial();
						break;
						case 7:
							power();
							break;
							case 8:
								square();
								break;
								case 9:
									squareroot();
									break;
									case 10:
										cube();
										break;
									/*	case 0:
											exist(0);
											break;*/
											default:
												printf("\n***%s****\n");
					
		}
	}
	return 0;
}

void addition(){
	printf("enter the number you want to add\n");
	int a, b;
	scanf("%d%d",&a,&b);
	printf("the sum of number are %d\n",a+b);
}
void substraction(){
	printf("enter the number to substract\n");
	int a, b;
	scanf("%d%d",&a,&b);
	printf("the substraction of number are %d\n",a-b);
}
void multiplicaliton(){
	printf("enter the number you want to multiplye\n");
	int a, b;
	scanf("%d%d",&a,&b);
	printf("the multiple of number are %d\n",a*b);
}
void division(){
	printf("enter the number you want to divide\n");
	int a, b;
	scanf("%d%d",&a,&b);
	printf("the division of number are %f\n",(float)a/(float)b);
}void modulus(){
	printf("enter the number you want to moduls\n");
	int a, b;
	scanf("%d%d",&a,&b);
	printf("the modulus of number are %d\n",a%b);
}
void factorial(){
	printf("enter the number you want to factorial\n");
	int n =0, i, factorial;
	scanf("%d",&n);
	factorial = 1;
	for(i=1; i<=n; i++){
		factorial= factorial*i; //factorial*=i; 
	}
	printf("the factorial of number %d are %d\n",n,factorial);
	
}
void power(){
	printf("enter the number you want to power\n");
	int x;
	int y;
	int result;
	scanf("%d%d",&x,&y);
	result=pow(x,y);
	printf("the result are %d\n",result);

}
void square(){
	printf("enter the number you want to square\n");
	double b;
	double p;
	scanf("%lf",&b);
	p=pow(b,2);
	printf("the square of number %lf are %lf\n", b, p);

}
void squareroot(){
	printf("enter the number you want to squareroot\n");
	double b;
	double s;
	scanf("%lf",&b);
	s = sqrt(b);
	printf("the squareroot of %lf number are %lf\n", b, s);
	
}
void cube(){
	printf("enter the number you want to cube\n");
	int b,p;
	scanf("%d",&b);
	 p= pow(b,3);
	printf("the cube of number %d are %d\n", b, p);
	
}


