1. (Problema 1020 - Idade em Dias)
#include <stdio.h>
int main() { int N; // Idade total em dias
// 1. Leitura do valor total em dias
scanf("%d", &N);

// 2. Cálculo e Impressão dos Anos
printf("%d ano(s)\n", N / 365);
N %= 365; // Atualiza N para os dias restantes após os anos

// 3. Cálculo e Impressão dos Meses
printf("%d mes(es)\n", N / 30);
N %= 30; // Atualiza N para os dias restantes após os meses

// 4. Impressão dos Dias (o que restou em N)
printf("%d dia(s)\n", N);

return 0;

}

2. (Problema 1019 - Conversão de Tempo)
#include <stdio.h>
int main() { int N; // Tempo total em segundos (Entrada)
// 1. Leitura do valor total em segundos
scanf("%d", &N);

// 2. Impressão do resultado no formato H:M:S
// H = N / 3600
// M = (N % 3600) / 60
// S = (N % 3600) % 60 (simplificado para N % 60, se M for calculado antes)
printf("%d:%d:%d\n", N / 3600, (N % 3600) / 60, N % 60);

return 0;

}

3. (Problema 1017 - Gasto de Combustível)
#include <stdio.h>
int main() { int T, V; // Tempo (T) e Velocidade Média (V)
// Leitura dos dois inteiros (tempo e velocidade)
scanf("%d %d", &T, &V);

// Impressão direta do resultado formatado: (T * V) / 12.0
// O 12.0 garante que a divisão seja de ponto flutuante.
// %.3f formata o resultado com 3 casas decimais.
printf("%.3f\n", (T * V) / 12.0);

return 0;

}

4.(Problema 1018 - Cédulas)
#include <stdio.h>
int main() { int N;
// 1. Leitura e Impressão do valor original
scanf("%d", &N);
printf("%d\n", N);

// 2. Decomposição (Divisão e Módulo) e Impressão

printf("%d nota(s) de R$ 100,00\n", N / 100);
N %= 100;

printf("%d nota(s) de R$ 50,00\n", N / 50);
N %= 50;

printf("%d nota(s) de R$ 20,00\n", N / 20);
N %= 20;

printf("%d nota(s) de R$ 10,00\n", N / 10);
N %= 10;

printf("%d nota(s) de R$ 5,00\n", N / 5);
N %= 5;

printf("%d nota(s) de R$ 2,00\n", N / 2);
N %= 2;

printf("%d nota(s) de R$ 1,00\n", N); // N / 1 é o próprio N

return 0;

}

5.(Problema 1017 - Gasto de Combustível)
#include <stdio.h>
int main() { int T, V; // Tempo (T) e Velocidade Média (V)
// Leitura dos dois inteiros (tempo e velocidade)
scanf("%d %d", &T, &V);

// Impressão direta do resultado formatado: (T * V) / 12.0
// O 12.0 garante que a divisão seja de ponto flutuante.
// %.3f formata o resultado com 3 casas decimais.
printf("%.3f\n", (T * V) / .0);

return 0;

}

6 . (Problema 1016 - Distância)
#include <stdio.h>
int main() { int D; // Distância de separação desejada (em Km) int tempo; // Tempo necessário (em minutos)
// 1. Leitura da distância D (um número inteiro)
scanf("%d", &D);

// 2. Cálculo do tempo: 2 minutos por quilômetro
// tempo = D * 2;
tempo = D * 2;

// 3. Impressão do resultado formatado: valor seguido de " minutos"
printf("%d minutos\n", tempo);

return 0;

}

7. (Problema 1015 - Distância Entre Dois Pontos)
#include <stdio.h>
int main() { // Declaração das coordenadas dos pontos P1 e P2 como doubles double x1, y1, x2,y2; double distancia;
// 1. Leitura dos valores de P1 (x1 y1) - Primeira linha
// Utilizamos %lf para ler doubles
scanf("%lf %lf", &x1, &y1);

// 2. Leitura dos valores de P2 (x2 y2) - Segunda linha
scanf("%lf %lf", &x2, &y2);

// 3. Cálculo da distância usando a fórmula: sqrt((x2-x1)^2 + (y2-y1)^2)
// pow(base, expoente) calcula a potência.
distancia = sqrt(pow(x2 - x1, 2) + pow(y2 - y1, 2));

// 4. Impressão do resultado formatado
// O modificador %.4f formata a saída com 4 casas decimais.
printf("%.4f\n", distancia);

return 0;

}

8. (Problema 1014 - Consumo)
1. #include <stdio.h>
int main() { int X; // Distância total percorrida (Km) double Y; // Total de combustível gasto (litros)
// 1. Leitura dos valores: um inteiro (%d) e um double (%lf)
scanf("%d %lf", &X, &Y);

// 2. Impressão do resultado formatado
// O cálculo (X / Y) é feito na hora.
// O modificador %.3f formata a saída com 3 casas decimais.
printf("%.3f km/l\n", X / Y);

return 0;

}

9. (Problema 1013 - O Maior)
2. #include <stdio.h>
int main() { int a, b, c, maiorAB, maior;
scanf("%d %d %d", &a, &b, &c);

maiorAB = (a + b + abs(a - b)) / 2;
maior = (maiorAB + c + abs(maiorAB - c)) / 2;

printf("%d eh o maior\n", maior);

return 0;

}

10.(Problemas 1012 - Área)
#include <stdio.h>
int main() { double A, B, C; double triangulo, circulo, trapezio, quadrado, retangulo; const double PI = 3.14159;
scanf("%lf %lf %lf", &A, &B, &C);

triangulo = (A * C) / 2.0;
circulo = PI * C * C;
trapezio = ((A + B) * C) / 2.0;
quadrado = B * B;
retangulo = A * B;

printf("TRIANGULO: %.3lf\n", triangulo);
printf("CIRCULO: %.3lf\n", circulo);
printf("TRAPEZIO: %.3lf\n", trapezio);
printf("QUADRADO: %.3lf\n", quadrado);
printf("RETANGULO: %.3lf\n", retangulo);

return 0;

}

11. (Problema 1011 - Esfera)
2. #include <stdio.h>
int main() { double R, volume; double pi = 3.14159;
scanf("%lf", &R);
volume = (4.0/3) * pi * (R * R * R);

printf("VOLUME = %.3lf\n", volume);
return 0;

}

12. (Problema 1010 - Cálculo Simples)
2. #include <stdio.h>
int main() { int cod1, cod2, qtd1, qtd2; double valor1, valor2, total;
// leitura dos dados da primeira peça
scanf("%d %d %lf", &cod1, &qtd1, &valor1);

// leitura dos dados da segunda peça
scanf("%d %d %lf", &cod2, &qtd2, &valor2);

// cálculo do total a pagar
total = (qtd1 * valor1) + (qtd2 * valor2);

// saída formatada com duas casas decimais
printf("VALOR A PAGAR: R$ %.2lf\n", total);

return 0;

}

13. (Problema 1009 - Salário com Bônus)
2. #include <stdio.h>
int main() { char nome[100]; double salario_fixo, total_vendas, total;
// Lê os dados de entrada
scanf("%s", nome);
scanf("%lf", &salario_fixo);
scanf("%lf", &total_vendas);

// Calcula o total (salário fixo + 15% das vendas)
total = salario_fixo + (total_vendas * 0.15);

// Imprime o resultado com duas casas decimais
printf("TOTAL = R$ %.2lf\n", total);

return 0;

}
14.(Problema 1008 - Salário)
#include <stdio.h>
int main() { int numero, horas; float valorHora, salario;
scanf("%d", &numero);
scanf("%d", &horas);
scanf("%f", &valorHora);

salario = horas * valorHora;

printf("NUMBER = %d\n", numero);
printf("SALARY = U$ %.2f\n", salario);

return 0;

}

15. (Problema 1007 - Diferença)
2. #include <stdio.h>
int main(void) { int A, B, C, D, DIFERENCA;
scanf("%d", &A);
scanf("%d", &B);
scanf("%d", &C);
scanf("%d", &D);

DIFERENCA = (A * B - C * D);

printf("DIFERENCA = %d\n", DIFERENCA);

return 0;

}

16. ( Problema 1006 - Média 2)
2. #include <stdio.h>
int main() { double A, B, C, media; scanf("%lf", &A); scanf("%lf", &B); scanf("%lf", &C);
media = (A * 2 + B * 3 + C * 5) / 10;

printf("MEDIA = %.1lf\n", media);

return 0;

}

17. (Problema 1005 - Média 1 )
2. #include <stdio.h>
int main() { double A, B, MEDIA; scanf("%lf", &A); scanf("%lf", &B);
MEDIA = (A * 3.5 + B * 7.5) / 11.0;

printf("MEDIA = %.5lf\n", MEDIA);

return 0;

}

18. ( Problema 1004 - Produto Simples)
#include <stdio.h> int main() { int A, B, PROD;
scanf("%d %d", &A, &B);

PROD = A * B;

printf("PROD = %d\n", PROD);
return 0;

}

19. (Problema 1003 - Soma Simples)
2. #include <stdio.h>
int main() {
int A, B, SOMA;

scanf("%d", &A);
scanf("%d", &B);

SOMA = A + B;

printf("SOMA = %d\n", SOMA);

return 0;

}

20. ( Problema 1001 - Extremamente Básico)
2. #include <stdio.h>
int main() { // Declaração das variáveis. int A, B, X;
// 1. Leitura da Entrada: Lê dois valores inteiros (A e B) da entrada.
// O scanf lerá os valores que o sistema de teste fornecer.
scanf("%d", &A);
scanf("%d", &B);

// 2. Cálculo: Realiza a soma de A e B e armazena em X.
X = A + B;

// 3. Impressão da Saída: Imprime o resultado no formato EXATO.
// "X = [valor]\n"
// Note: X maiúsculo, um espaço antes e um depois do sinal de igual, 
// e o "\n" para a quebra de linha.
printf("X = %d\n", X);

return 0;

}