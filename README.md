#include <stdio.h>
#include <ctype.h>

int main() {
    char letra;

    printf("Digite uma letra: ");
    scanf(" %c", &letra);

   
    if (letra) {
       
        if (isupper(letra)) {
            printf("A letra digitada ja e maiuscula.\n");
        } else {
            printf("A letra digitada e minuscula.\n");
        }

       
        printf("Minuscula: %c\n", tolower(letra));
        printf("Maiuscula: %c\n", toupper(letra));
    } else {
        printf("O caractere digitado nao e uma letra.\n");
    }

    return 0;
}
