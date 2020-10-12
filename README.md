# Alguns-Exercicios-basicos-do-primeiro-semestre-da-faculdade-usando-IF

Exercicio 01

#include <stdio.h>
#include <stdlib.h>
#include <locale.h>

int main()
{

  int num1, num2;
  setlocale(LC_ALL,"portuguese");

 printf("digite 2 numeros inteiros: ");

 scanf("%d%d",&num1, &num2);


 if(num1 > num2)

 {

 printf("%d", num1);

 }

 else

 printf("");




    return 0;
}


Exercicio =02

#include <stdio.h>
#include <stdlib.h>
#include <locale.h>

int main()
{

  int num1;
  setlocale(LC_ALL,"portuguese");

 printf("digite sua data de nascimento: ");

 scanf("%d",&num1);


 if(num1 <= 2004)

 {

 printf("\n*Você podera votar esse ano*\n");

 }

 else

 printf("");




    return 0;
}

exercicio = 03 Senha

#include <stdio.h>
#include <stdlib.h>

int main()
{



 int num1;

 printf("digite a senha ");

 scanf("%d",&num1);
 

 if(num1 != 1234)

 {

 printf("ACESSO NEGADO");

 }

 else

 printf("ACESSO PERIMITIDO");


}

 exercicio = 04 maças

#include <stdio.h>
#include <stdlib.h>
#include <locale.h>

int main()
{
	setlocale(LC_ALL, "portuguese");



 float macascompradas, resultado ;

 printf("Quantas maças você comprou");

 scanf("%f",&macascompradas);


 if(macascompradas <12)

 {

   resultado = macascompradas * 0.30;
   printf(" você vai pagar%0.2f", resultado);
 }

 else

   resultado = macascompradas * 0.25;
   printf(" você vai pagar%0.2f", resultado);


}

exercicio 05

#include <stdio.h>

int main() {
    int a, b, c;
    printf("Digite 3 numeros:\n");
    scanf("%d %d %d", &a, &b, &c);
    if (a > c) {
        int tmp = c;
        c = a;
        a = tmp;
    }
    if (a > b) {
        int tmp = b;
        b = a;
        a = tmp;
    }
    if (b > c) {
        int tmp = c;
        c = b;
        b = tmp;
    }
    printf("%d %d %d", a, b, c);
}

Exercicio = 06

#include<stdio.h>
#include<stdlib.h>
#include<conio.h>
#include<locale.h>


int main(){

setlocale(LC_ALL,"portuguese");

float altura, total;

int sexo;

printf("Exercicio 6!");

printf("\n\nEscreva sua altura:");
scanf("%f", &altura);

fflush(stdin);

printf("\n\nSe seu genero for masculino, tecle 1. Se feminino 2:");
scanf("%d",&sexo);



fflush(stdin);

if(sexo == 1){

total = ((72.7*altura)-58);

printf("\nSeu peso ideal: %.2f", total);

 }

 else

 {

 total = (62.1 * altura)-47.7;

printf("\nSeu peso ideal: %.2f", total);

}

 getch();

 }



Exercicio 07


#include<stdio.h>
#include<stdlib.h>
#include<conio.h>
#include<locale.h>
int main(){ setlocale(LC_ALL,"");
float lado, ladop, tamanho, altura, base, total;
printf("\n\n\nEsvreva o Nº de LADOS do Poligono: ");
scanf("%f",&lado);
if(lado==3)
{
printf("\nDigit a Altura do Triangulo: ");
scanf("%f",&altura); printf("\nDigit a Base do Triangulo: ");
scanf("%f",&base); total = (base*altura)/2; printf("\nA area do Triangulo é = %.2f",total);
}
else if(lado == 4)
{ printf("\nDigite a Base do Quadrado: ");
scanf("%f",&base); printf("\nDigite a Altura do Quadrado: ");
scanf("%f",&altura); total = base*altura; printf("\nA area do Quadrado é = %.2f",total); }
else if(lado == 5)
{ printf("\nDigite o Tamanho do Lado do Pentagono: ");
scanf("%f", &ladop); printf("\nDigite a Altura do Pentagono: ");
scanf("%f", &altura); total = (ladop*5)*altura; printf("\nA area do Pentagono é = %.2f",total); }
else
{
printf("forma não localizada!");
}
getch(); }

exercicio 09

#include <stdio.h>
#include <stdlib.h>
#include <locale.h>

int main()
{

  int num1, num2, num3;
  setlocale(LC_ALL,"portuguese");

 printf("digite 3 numeros inteiros: ");

 scanf("%d%d%d",&num1, &num2, &num3);


 if(num1 > num2 && num1 > num3 )

 {

 printf("\nO maior numeero digitado foi %d\n", num1);

 }

 else if(num2 > num3 && num2 > num1)
 {



 printf("\nO maior numero digitado foi %d\n",num2 );
 }
 else if (num3 > num2 && num3 > num1)
 {


 printf("\nO maior numero digitado foi %d\n", num3);
 }



    return 0;
}

exercicio = 10

#include<stdio.h>
#include<stdlib.h>
#include<conio.h>
#include<locale.h>

int main(){

 setlocale(LC_ALL,"portuguese");



int lado1, lado2, lado3;
 float num1, num2, num3;

 printf("\nDigite o 1º Lado: ");
 scanf("%d",&lado1);

 printf("\nDigite o 2º Lado: ");
 scanf("%d",&lado2);

 printf("\nDigite o 3º Lado: ");
 scanf("%d",&lado3);

 num1 = lado1+lado2;
 num2 = lado1+lado3;
 num3 = lado2+lado3;

 if (num1>lado3 && num2>lado2 && num3>lado1)
 {
   if (lado1==lado2 && lado2==lado3)
 {
	printf("\nEste é um Triângulo Equilatero");
 }

else if(lado1==lado2 || lado1==lado3 || lado2==lado3)//"|| = ou"

 {
	printf("\nEste é um Triângulo Isoceles!");
 }

else if(lado1!=lado2 && lado2!=lado3 && lado1!=lado3)

 {
	printf("\nEste é um Triângulo Escaleno");
 }
}
 else
 {
 	printf("\nEle não é um Triangulo");
 }


 getch();
 }


Exercicio = 11

#include<stdio.h>
#include<stdlib.h>
#include<conio.h>
#include<locale.h>

int main(){

 setlocale(LC_ALL,"");

int angulo1, angulo2, angulo3;
 float num1;

 printf("\nDigite o 1º Lado: ");
 scanf("%d",&angulo1);

 printf("\nDigite o 2º Lado: ");
 scanf("%d",&angulo2);

 printf("\nDigite o 3º Lado: ");
 scanf("%d",&angulo3);

num1= angulo1+angulo2+angulo3;

 if (num1==180)
 {
   if (angulo1==90 ||angulo2==90 || angulo3==90)
 {
	printf("\nEste é um Triângulo Retangulo.");
 }

else if(angulo1>90 ||angulo2>90 || angulo3>90)

 {
	printf("\nEste é um Triângulo Abtusangulo.");
 }

else if(angulo1<90 && angulo2<90 && angulo3<90)

 {
	printf("\nEste é um Triângulo Acutângulo.");
 }
}
 else
 {
 	printf("\nEle não é um Triangulo.");
 }

 getch();
 }
