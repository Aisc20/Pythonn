# C estudos

#include <stdio.h>
#include <stdlib.h>

int main()
{
    float a, b; 
    int num;
    
    printf("Infome dois numeros:");
    scanf("%f %f", &a, &b);
    
    printf("informe qual operação deve ser realizada \n");
    printf("1. soma \n");
    printf("2. sub \n");
    printf("3. multiplicação \n");
    printf("4. divisão \n");
    scanf("%d", &num);
    
    switch(num){
        case 1:
            printf("a soma eh %.1f", a+b);
            break;
        case 2:
            printf("a sub eh %.1f", a-b);
            break;
        case 3:
            printf("a mul eh %.1f", a*b);
            break;
        case 4:
            if(b){
            printf("a div eh %.2f", a/b);
            break;
            }
            else{
                printf("nao eh possivel realizar a divisao");
                break;
            }
        default:
            printf("esse numero nao eh valido");
    }
    
    return 0;
}
