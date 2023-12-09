#include <stdio.h>
#include <string.h>


int main() {
  char comida[30];
  char bebida[30];
  float valorcomida=0 , valorsuco=0 , final;
  
   printf("O que voce deseja comer? ");
  
   scanf("%s", comida);
  
   printf("e para beber? ");

   scanf("%s", bebida);
  
  // Comparação da string inserida com "lasanha"
 if(strcasecmp (comida, "lasanha") ==0)
     {valorcomida = valorcomida + 8.00;}
      else if (strcasecmp (comida, "estrogonofe") ==0)
        {valorcomida = valorcomida + 11.00;}
    //strcasecmp =  é usada para realizar a comparação de strings sem levar em conta a diferença entre maiúsculas e minúsculas. Esta função compara duas strings e retorna um número inteiro que indica o relacionamento entre elas
  if(strcasecmp (bebida, "refrigerante") ==0)
     {valorsuco = valorsuco + 3.00;}
       else if(strcasecmp (bebida, "suco") ==0)
        {valorsuco = valorsuco + 2.50;}

final = valorcomida + valorsuco;
   printf ("sua conta e de %.2f\n" , final);
  
  return 0;
}
