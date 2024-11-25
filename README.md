#include <stdio.h>

int main(){
    
    int num[10];
    int i = 0, maior, menor; 
    
    for (i = 0; i < 10; i++){
        
        printf("Digite o %d° número inteiro: ", i + 1);
        scanf("%d", &num[i]);
        
        if(i == 0){
            maior = num[i];
        }
        else if (num[i] > maior) {
             maior = num[i];
        }
        else{
            if (num[i] < maior) {
                menor = num[i];
            }
        }
        
    }
    printf("O maior número inserido foi: %d\n", maior);
    printf("O menor número inserido foi: %d\n", menor);
    

    return 0;
}
