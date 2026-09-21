# entrega
#include <stdio.h>

int main() {
int mat[3][3];
int i, j;
int iteracao = 1;

// 1 e 2. Declarar e preencher com dois for aninhados
int valores[3][3] = {
{5, 8, 12},
{15, 20, 25},
{30, 35, 40}
};

printf("Preenchendo a matriz:\n");
for(i = 0; i < 3; i++) {
for(j = 0; j < 3; j++) {
mat[i][j] = valores[i][j];
printf("Iteracao %d: i=%d j=%d -> mat[%d][%d] = %d\n",
iteracao, i, j, i, j, mat[i][j]);
iteracao++;
}
}

// 3. Exibir a matriz organizada em linhas e colunas
printf("\nMatriz 3x3 exibida:\n");
for(i = 0; i < 3; i++) {
for(j = 0; j < 3; j++) {
printf("%4d", mat[i][j]);
}
printf("\n");
}

return 0;
}
