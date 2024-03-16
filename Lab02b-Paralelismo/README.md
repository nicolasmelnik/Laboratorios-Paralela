# Lab02b - Programação Paralela!

Este é o README para o "Lab02b - Programação Paralela!", desenvolvido em linguagem C. Este documento contém instruções detalhadas sobre como compilar, executar e verificar os resultados do programa entregue.

## Integrantes do grupo
- Felipe Mazzeo Barbosa.
- Matteo Domiciano Varnier.
- Nicolas Fernandes Melnik.

## Como Compilar

Para compilar os programas do laboratório no Linux, siga os passos abaixo:
1. Abra o terminal.
2. Navegue até o diretório do projeto.
3. Para cada programa que deseja compilar, execute o seguinte comando, substituindo [NomeArquivo] pelo respectivo nome do programa: `gcc -o [NomeArquivo].bin [NomeArquivo].c -lpthread`.
4. Por exemplo: você quer compilar o multiplicacaoMatrizes.c, basta executar o comando `gcc -o multiplicacaoMatrizes.bin multiplicacaoMatrizes.c -lpthread`. Assim, é gerado um executável chamado multiplicacaoMatrizes.bin no diretório atual.

## Como Executar

Após compilar o projeto, siga estas etapas para executá-lo:
1. No terminal, certifique-se de estar no diretório onde o executável foi gerado.
2. Execute o seguinte comando: `time taskset -c 0 ./[NomeArquivo].bin`.
3. No comando acima, basta substituir `[NomeArquivo]` pelo nome do arquivo executável gerado pela compilação.
4. No comando utilizamos `time` para que seja possível visualizar o tempo de execução sem afetar o programa em si.
5. No comando, também utilizamos `taskset - c 0`, para especificar quais núcleos estamos utilizando na execução. Esse comando pode ser adaptado da maneira que preferir, mas para essa atividade utilizamos:
- taskset - c 0
- taskset - c 0, 1
- taskset - c 0, 1, 2, 3
- taskset - c 0, 1, 2, 3, 4, 5
- taskset - c 0, 1, 2, 3, 4, 5, 6, 7

## Resultados
Primeiramente, como solictado pelo professor, executamos o comando `cat /proc/cpuinfo` para verificar a configuração do processador utilizado, como é mostrado na imagem a seguir:

![CPU info](https://github.com/nicolasmelnik/Laboratorios-Paralela/assets/117850844/c99daa7a-5aaa-4718-b0a7-35b94a2bf08d)

Construa uma solução paralela e responda às seguintes questões:

1. Qual o tempo de execução serial e paralelo para 1, 2, 4, 6 e 8 processadores? Desenhe um gráfico contendo todos os tempos de execução

2. Qual o speedup para 1, 2, 4, 6 e 8 processadores? Desenhe um gráfico mostrando os diferentes valores de speedup.

3. Como você acha que poderia melhorar o seu algoritmo para obter maior benefício com o paralelismo?Para provar seu ponto, refaça a solução com essa abordagem e construa um novo gráfico de speedup para 1, 2, 4, 6 e 8 processadores.
