#include <stdio.h>
#include <math.h>

int main(void) {

int Opcao;
char Nome[100];

//Apresentação do autor  
printf("Nome: Rodrigo da Silva Machado\nMatricula:202221556\nCurso:Superior de Tecnologia em Ciência de Dados\n" );

//Solicitar o nome do usuário
printf("\nQual o seu nome?\n");
scanf("\n%s",Nome);

system("clear");

//Manu para escolha 
printf("\nMenu:\n");
printf("\nOlá %s digite a opção desejada:", Nome);
printf("\n 1 - Raíz Quadrada ");
printf("\n 2 - Soma ");
printf("\n 3 - Multiplicação ");
printf("\n 4 - Divisão ");
printf("\n 5 - Potencial ");
printf("\n 6 - Fechar Programa\n ");
//Escolha da opção  
scanf("%d",&Opcao);

  switch (Opcao){
//Raiz Quadrada
    case 1:{
    system("clear");
   float Num1;   
   printf("\nDigite o número para calcular:\n");
   scanf("%f",&Num1); 
   float Raiz = sqrt(Num1);
  printf("A raiz quadrada do número digitado é: %.3f\n", Raiz);
     break; 
           }

    
    case 2:{
       system("clear");
      int Soma1;
      int Soma2;
//Soma
  printf("\nDigite um número para calcular:\n");
      scanf("%d", &Soma1);
  printf("\nDigite o segundo número para calcular:\n");
      scanf("%d", &Soma2);
    
      int Resultadosoma = Soma1 + Soma2;
        printf("\nO resultado da soma é= %d", Resultadosoma);
      return 0;
        }
    case 3:{
       system("clear");
    float Multi1;
    float Multi2;
//Multiplicação
      printf("\nDigite um número para calcular:\n");
      scanf("%f", &Multi1);
      printf("\nDigite um número para calcular:\n");
      scanf("%f", &Multi2);
      float ResultadoMulti = Multi1*Multi2;
      printf("\nO resultado da soma é= %.2f", ResultadoMulti);
      return 0;
    }
    case 4:{
       system("clear");
    float Divi1;
    float Divi2;
  //Divisão
      printf("\nDigite um número para calcular:\n");
      scanf("%f", &Divi1);
      printf("\nDigite um número para calcular:\n");
      scanf("%f", &Divi2);
      
      float ResultadoDivi = Divi1*Divi2;
      printf("\nO resultado da soma é= %.2f", ResultadoDivi);
      return 0;
    }
      case 5:{
         system("clear");
    double Poten1;
    double Poten2;
//Potencia
      printf("\nDigite um número para calcular:\n");
      scanf("%lf", &Poten1);
       printf("\nDigite um número para calcular:\n");
      scanf("%lf", &Poten2);
      
      double Resultadopoten = pow(Poten1,Poten2);
      printf("\nO resultado da soma é= %lf", Resultadopoten);
        return 0;
    }
    case 6:{
      //encerrar
       system("clear");
    printf("\nAté logo %s!", Nome);
      break;      
    }
    system("clear");
    
    default:
    printf("Opção invalida.");

      }


  }
    
  







