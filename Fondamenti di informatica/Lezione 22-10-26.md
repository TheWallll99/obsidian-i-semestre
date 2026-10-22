## PUNTATORI
Un puntatore è una variabile che punta all'indirizzo di un'altra variabile. Occupa 8 byte e indica semplicemente il numero dell'indirizzo della variabile a cui punta. Si dichiarano con un asterisco. Modificando il puntatore con l'asterisco si modifica la variabile a cui punta. Quando aggiungiamo un valore ad un puntatore stiamo modificando quel puntatore aggiungendogli tanti byte quanti ne richiede il suo tipo.

#### Codici:
#include<stdio.h>

int main(){

    signed char ch = 5; //signed char si riferisce a un numero che è considerato carattere

    signed char *add = &ch; // add è un PUNTATORE che PUNTA all'indirizzo di a

    int a = 10;

    int b = 100;

    int *int_pnt=NULL; // NULL vale 0

    int_pnt=&a;

    printf("\nContenuto del puntatore: %lld", int_pnt);

    int_pnt = int_pnt+1;

    printf("\nContenuto del puntatore dopo modifica: %lld", int_pnt);

    char array[5] = {'a','b','c','d','e'};

    char *arr_pnt = array;

    printf("\nContenuto del puntatore all'array di caratteri: %lld", arr_pnt);

    printf("\n%c",*arr_pnt);//così facendo si stampa la variabile a cui punta, in questo caso a

    return 0;

}