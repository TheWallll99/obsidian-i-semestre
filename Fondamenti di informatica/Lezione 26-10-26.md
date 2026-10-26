## ARRAY DI PUNTATORI
Ogni casella dell'array contiene un puntatore, e possiamo avere anche array di array (le matrici sostanzialmente), in ognuna delle caselle dell'array ci sono altri array. Ad esempio, mat$[2][4]$ indica la seconda riga e la quarta colonna. La disposizione della memoria però non è bidimensionale, gli array sono disposti uno dopo l'altro. Quando eseguo mat$[1]$ = $*$(mat+1), in memoria, sto avanzando di un intero array.
#### Codice:
#include<stdio.h>

int main(){

    int A[5][3];

    int B[3][5];

    int c=1;

    for(int i=0;i<5;i++){

        for(int j=0;j<3;j++){

            A[i][j]=c;

            c++;

        }

        c+=6;

    }

    for (int i=0;i<3;i++){

        for(int j=0;i<5;i++){

            B[i][j]=A[j][i];

        }

    }

    for (int i=0;i<5;i++){

        for(int j=0;i<3;i++){

            printf("%d ",A[i][j]);

        }

        printf("\n");

    }

    for (int i=0;i<3;i++){

        for(int j=0;i<5;i++){

            printf("%d ",B[i][j]);

        }

        printf("\n");

    }

    return 0;

}