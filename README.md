# rocksdxebec

#include <stdio.h>
#include <stdlib.h>
/* Faça um codigo que leia em ateh uma matriz 10x10 e defina
   o maior, menor e a media encontrada na matriz */
int main(void)
{
    float M[3][3];
    int j = 0;
    int k = 0;
    float maior = 0;
    float menor = 999999;
    float soma = 0;

/*Preenchimento dos valores contidos na matriz*/
    for(j = 0; j < 3; ++j)
        {
        for(k = 0; k<3; ++k)
            {
            printf("\n Digite um numero \n");
            scanf("%f", &M[j][k]);
            soma = soma+M[j][k];
            }

        }

/*Condição para ver se eh maior ou menor */

    for(j = 0; j<3; ++j)
        {
            for(k = 0; k<3; ++k)
            {
                if(M[j][k]>maior)
                    maior =M[j][k];
            }
        }
    for(j = 0; j<3; ++j)
    {
        for(k=0; k<3; ++k)
        {
            if(M[j][k]<menor)
                menor = M[j][k];
        }
    }

    printf("\n Maior=%.2f, Menor=%.2f, Media=%.2f", maior,menor,soma/9);

    return 0;
}




















