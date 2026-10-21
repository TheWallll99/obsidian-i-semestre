## ARRAY
Gli array sono insiemi di elementi che occupano spazi di memoria vicini tra di loro, come dei pacchetti. Non vengono effettuati controlli sull'indice utilizzato, quindi è facile accedere a zone di memoria non allocate semplicemente inserendo un indice troppo alto.
Gli array non possono essere trattati come variabili a loro stanti, ma hanno bisogno di essere accompagnati dall'indicatore di indice $[$ $]$
## STRINGHE
Le stringhe sono insiemi di caratteri. La differenza tra esse e un comune array di caratteri è che le stringhe hanno un carattere extra chiamato **terminatore di stringa** o **carattere di terminazione** (\0).

### codice:
#include<stdio.h>

#include<string.h> //per usare le cose strane con le stringhe pazze

int main(){

    char array_char[]={'H','e','l','l','o'};

    char str1[]="Hola";

    // si può sondare la dimensione di un array tramite l'operatore sizeof()

    // e la lunghezza dividendo la dimensione dell'array per la

    // dimensione di un singolo carattere

    int size_char=sizeof(array_char)/sizeof(char);

    int size2=sizeof(str1)/sizeof(char);

    printf("la dimensione di %s \212: %d \n", array_char, size_char);

    printf("la dimensione di %s \212: %d \n", str1, size2);

    int leng=strlen(str1); //restituisce la lunghezza senza carattere di terminazion

    printf("la dimensione di %s, ancora una volta, \212: %d", str1, leng);

    char nome[100];

    printf("\n Come ti chiami? ");

    scanf ("%s", nome);

    printf("\n Ah, ti chiami %s, mi dispiace per te", nome);

    return 0;

}