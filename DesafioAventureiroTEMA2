#include <stdio.h>
#include <stdlib.h>

// Função principal
int main() {
    // Declaração de variáveis para armazenar dados das cartas
    char estado1[20], estado2[20];
    char codigo1[20], codigo2[20];
    char nome1[20], nome2[20];
    int populacao1, populacao2;
    float area1, area2;
    float PIB1, PIB2;
    int pturistico1, pturistico2;
    float densidadepo1, densidadepo2;
    float pibpercapita1, pibpercapita2;
    float superpoder1, superpoder2;
    int comparacao;
    int opcao;

    // Coleta de dados da CARTA 1
    printf("--- BORA PARA A COLETA DE DADOS DA CARTA! ---\n");
    printf("--- DIGITE AS INFORMAÇÕES DA CARTA 1 ---\n");

    printf("Digite o estado: ");
    scanf("%s", estado1);
    printf("Digite o código da carta: ");
    scanf("%s", codigo1);
    printf("Digite o nome da cidade: ");
    scanf("%s", nome1);
    printf("Digite a população: ");
    scanf("%d", &populacao1);
    printf("Digite a área: ");
    scanf("%f", &area1);
    printf("Digite o PIB: ");
    scanf("%f", &PIB1);
    printf("Digite o número de pontos turísticos: ");
    scanf("%d", &pturistico1);

    // Cálculo de dados derivados da carta 1
    densidadepo1 = (float)populacao1 / area1;
    pibpercapita1 = (float)PIB1 / populacao1;
    superpoder1 = (float)populacao1 + area1 + PIB1 + (1.0 / densidadepo1) + pibpercapita1;

    printf("\n");

    // Coleta de dados da CARTA 2
    printf("--- DIGITE AS INFORMAÇÕES DA CARTA 2 ---\n");

    printf("Digite o estado: ");
    scanf("%s", estado2);
    printf("Digite o código da carta: ");
    scanf("%s", codigo2);
    printf("Digite o nome da cidade: ");
    scanf("%s", nome2);
    printf("Digite a população: ");
    scanf("%d", &populacao2);
    printf("Digite a área: ");
    scanf("%f", &area2);
    printf("Digite o PIB: ");
    scanf("%f", &PIB2);
    printf("Digite o número de pontos turísticos: ");
    scanf("%d", &pturistico2);

    // Cálculo de dados derivados da carta 2
    densidadepo2 = (float)populacao2 / area2;
    pibpercapita2 = (float)PIB2 / populacao2;
    superpoder2 = (float)populacao2 + area2 + PIB2 + (1.0 / densidadepo2) + pibpercapita2;

    printf("\n");

    // Menu de comparação
    printf("--- COMPARAÇÃO DAS CARTAS ---\n");
    printf("1 - Comparar categoria isolada\n");
    printf("2 - Comparar superpoder\n");
    printf("Escolha uma opção: \n");
    scanf("%d", &comparacao);

    printf("\n");

    // Estrutura switch para decidir o tipo de comparação
    switch (comparacao) {
        case 1:
            // Submenu para escolher o atributo específico a comparar
            printf("--- QUAL CATEGORIA DESEJA COMPARAR? ---\n");
            printf("1 - População\n");
            printf("2 - Área\n");
            printf("3 - PIB\n");
            printf("4 - Pontos Turísticos\n");
            printf("5 - Densidade Populacional\n");
            printf("6 - PIB Percapita\n");
            printf("Escolha uma opção: \n");
            scanf("%d\n", &opcao);

            // Comparações com base na opção escolhida
            if (opcao == 1) {
                printf("População carta 1: %d\n", populacao1);
                printf("População carta 2: %d\n", populacao2);
                if (populacao1 > populacao2) {
                    printf("### CARTA 1 VENCEU ###\n");
                } else if (populacao2 > populacao1) {
                    printf("### CARTA 2 VENCEU ###\n");
                } else {
                    printf("Empate!\n");
                }
            }

            if (opcao == 2) {
                printf("Área carta 1: %.2f\n", area1);
                printf("Área carta 2: %.2f\n", area2);
                if (area1 > area2) {
                    printf("### CARTA 1 VENCEU ###\n");
                } else if (area2 > area1) {
                    printf("### CARTA 2 VENCEU ###\n");
                } else {
                    printf("Empate!\n");
                }
            }

            if (opcao == 3) {
                printf("PIB carta 1: %.2f\n", PIB1);
                printf("PIB carta 2: %.2f\n", PIB2);
                if (PIB1 > PIB2) {
                    printf("### CARTA 1 VENCEU ###\n");
                } else if (PIB2 > PIB1) {
                    printf("### CARTA 2 VENCEU ###\n");
                } else {
                    printf("Empate!\n");
                }
            }

            if (opcao == 4) {
                printf("Ponto Turístico carta 1: %d\n", pturistico1);
                printf("Ponto Turístico carta 2: %d\n", pturistico2);
                if (pturistico1 > pturistico2) {
                    printf("### CARTA 1 VENCEU ###\n");
                } else if (pturistico2 > pturistico1) {
                    printf("### CARTA 2 VENCEU ###\n");
                } else {
                    printf("Empate!\n");
                }
            }

            if (opcao == 5) {
                printf("Densidade Populacional carta 1: %.2f\n", densidadepo1);
                printf("Densidade Populacional carta 2: %.2f\n", densidadepo2);
                // REGRA INVERTIDA: MENOR densidade vence
                if (densidadepo1 < densidadepo2) {
                    printf("### CARTA 1 VENCEU ###\n");
                } else if (densidadepo2 < densidadepo1) {
                    printf("### CARTA 2 VENCEU ###\n");
                } else {
                    printf("Empate!\n");
                }
            }

            if (opcao == 6) {
                printf("PIB percapita carta 1: %.2f\n", pibpercapita1);
                printf("PIB percapita carta 2: %.2f\n", pibpercapita2);
                if (pibpercapita1 > pibpercapita2) {
                    printf("### CARTA 1 VENCEU ###\n");
                } else if (pibpercapita2 > pibpercapita1) {
                    printf("### CARTA 2 VENCEU ###\n");
                } else {
                    printf("Empate!\n");
                }
            }
            break;

        case 2:
            // Comparação baseada no "superpoder" calculado
            printf("--- COMPARAÇÃO DE SUPERPODER ---\n");
            printf("Superpoder carta 1: %.2f\n", superpoder1);
            printf("Superpoder carta 2: %.2f\n", superpoder2);
            if (superpoder1 > superpoder2) {
                printf("### CARTA 1 VENCEU ###\n");
            } else if (superpoder2 > superpoder1) {
                printf("### CARTA 2 VENCEU ###\n");
            } else {
                printf("Empate!\n");
            }
            break;

        default:
            // Caso haja uma opção inválida
            printf("Opção inválida.\n");
            break;
    }

    return 0;
}
