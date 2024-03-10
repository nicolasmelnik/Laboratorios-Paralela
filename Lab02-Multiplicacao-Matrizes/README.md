# Lab02 - Programação matriz-vetor!

Este é o README para o "Lab02 - Programação matriz-vetor!", desenvolvido em linguagem C. Este documento contém instruções detalhadas sobre como compilar, executar e verificar os resultados do programa entregue.

## Integrantes do grupo
- Felipe Mazzeo Barbosa.
- Matteo Domiciano Varnier.
- Nicolas Fernandes Melnik.

## Como Compilar

Para compilar o programa no Linux, siga os passos abaixo:
1. Abra o terminal.
2. Navegue até o diretório do projeto.
3. Para compilar o programa, execute o seguinte comando: `gcc -o multiplicacaoMatrizes.bin multiplicacaoMatrizes.c -lpthread`.
4. Assim, é gerado um executável chamado `multiplicacaoMatrizes.bin` no diretório atual.

## Como Executar

Após compilar o programa, siga estas etapas para executá-lo:
1. No terminal, certifique-se de estar no diretório onde o executável foi gerado.
2. Execute o seguinte comando: `./multiplicacaoMatrizes.bin >> resultado.txt`.
3. Com o comando acima, no arquivo `resultado.txt` será exibido o resultado da execução do programa.

## Resultados
O resultado esperado (multiplicação correta de matrizes) para esta atividade foi alcançado. Para comprovar que nosso código foi compilado e executado no ambiente da AWS (conforme solicitado pelo professor), apresentamos a seguinte imagem:

![Lab02a](https://github.com/nicolasmelnik/Laboratorios-Paralela/assets/117850844/923aa5a9-f121-4efe-af67-cd9eb15ea2f4)

Para visualizar a saída do código, basta olhar o arquivo `resultado.txt`, pois fica melhor a visualização da Matriz resultado. Abaixo, temos uma imagem que serve como comprovação que nosso resultado está correto, pois utilizamos uma calculadora de matrizes online, onde digitamos a matriz A e elevamos ela ao quadrado. Elevamos ela ao quadrado, pois como a matriz B é idêntica a matriz A, é obtido o mesmo resultado, ou seja, AxB é igual a A^2.

![Lab02b](https://github.com/nicolasmelnik/Laboratorios-Paralela/assets/117850844/e77efbff-e1a5-4388-96c4-1043629b2a62)
