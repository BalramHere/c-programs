# c-programs

#include<stdio.h>
    #define PRINT(x) ("x") 
8int main() 
{ 
printf("%s",PRINT(x)); 
return 0; 
} 
#include <stdio.h> 

#define MACRO(num, str) ({ \ 
			printf("%d", num);\ 
			printf(" is");\ 
			printf(" %s number", str);\ 
			printf("\n");\ 
		} )

int main(void) 
{ 
	int num; 

	printf("Enter a number: "); 
	scanf("%d", &num); 

	if (num & 1) 
		MACRO(num, "Odd"); 
	else
		MACRO(num, "Even"); 

	return 0; 
} 
*/
#include <stdio.h> 

#define OFFSETOF(TYPE, ELEMENT) ((size_t)&(((TYPE *)0)->ELEMENT)) 

typedef struct PodTag 
{ 
int   i; 
double d; 
char  c; 
} PodType; 

int main() 
{ 
printf("%d", OFFSETOF(PodType, c) ); 
	
getchar(); 
return 0; 
} 
