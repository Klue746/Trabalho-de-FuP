#include <stdio.h>
#include <stdlib.h>
#include <locale.h>

int main() {
    int opcao;
    setlocale(LC_ALL, "Portuguese");

    do {
        system("clear"); 

        printf("=== MENU DE OPCOES ===\n");
        printf("[1] Saldo atual\n");
        printf("[2] Entrada\n");
        printf("[3] Saída\n");
        printf("[4] Saída\n");
        printf("[5] Saldo do mês\n");
        printf("[6] Categorias disponíveis\n");
        printf("[7] CDI\n");
        printf("[8] Dívidas\n");
        printf("[9] Meta\n");
        printf("[0] Sair\n");
        printf("Escolha uma opcao: ");
        scanf("%d", &opcao);

        switch (opcao) {
            case 1:
                printf("\nVoce escolheu o saldo atual.\n");
                break;
            case 2:
                printf("\nVoce escolheu a Entrada.\n");
                break;
            case 3:
                printf("\nVoce escolheu a Saída.\n");
                break;
            case 4:
                printf("\nVoce escolheu a Saída.\n");
                break;
            case 5:
                printf("\nVoce escolheu o saldo do mês.\n");
                break;
            case 6:
                printf("\nVoce escolheu as categorias disponíveis.\n");
                break;
            case 7:
                printf("\nVoce escolheu o CDI.\n");
                break;
            case 8:
                printf("\nVoce escolheu as dívidas.\n");
                break;
            case 9:
                printf("\nVoce escolheu a Meta.\n");
                break;
            case 0:
                printf("\nSaindo do programa...\n");
                break;
            default:
                printf("\nOpcao invalida! Tente novamente.\n");
        }

        if (opcao != 0) {
            printf("\nPressione ENTER para continuar...");
            getchar();
            getchar(); 
        }

    } while (opcao != 0);

    return 0;
}
