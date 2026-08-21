# ED2 — Sorting — Lista 01

Este repositório corresponde à **primeira etapa da atividade prática da disciplina de Estrutura de Dados II**, contendo o código-fonte dos exercícios propostos sobre algoritmos de ordenação.

O projeto foi desenvolvido em **C++** e utiliza **CMake** para organização, compilação e execução dos arquivos.

## Objetivos

A atividade tem como objetivo praticar a implementação e o funcionamento de algoritmos clássicos de ordenação, incluindo:

* Bubble Sort
* Selection Sort
* Insertion Sort
* Ordenação crescente e decrescente
* Controle de trocas
* Contagem de deslocamentos
* Manipulação de strings e vetores

## Tecnologias utilizadas

* C++
* CMake
* CLion
* Git
* GitHub

## Estrutura do projeto

```text
ed2-elementary-sorting-list01-cpp/
├── CMakeLists.txt
├── README.md
├── main.cpp
└── src/
    ├── Exer01_BubbleSortString.cpp
    ├── Exer02_SelectionSortDescending.cpp
    ├── Exer03_SelectionSortKSwaps.cpp
    ├── Exer04_InsertionSortShiftCount.cpp
    └── Exer05_InsertionSortDescendingTail.cpp
```

Cada exercício está localizado em seu próprio arquivo `.cpp` e possui um executável independente configurado no `CMakeLists.txt`.

## Exercícios

### Exercício 01 — Bubble Sort em String

Implementação do algoritmo **Bubble Sort** para ordenar os caracteres de uma string em ordem crescente.

Exemplo:

```text
Entrada:
patrocinio

Saída:
aciinooprt
```

### Exercício 02 — Selection Sort Decrescente

Implementação do algoritmo **Selection Sort** para ordenar os elementos em ordem decrescente.

### Exercício 03 — Selection Sort com K trocas

Variação do **Selection Sort** na qual a quantidade de trocas realizadas durante o processo de ordenação é limitada.

### Exercício 04 — Insertion Sort com contagem de deslocamentos

Implementação do **Insertion Sort** com contagem da quantidade de deslocamentos realizados durante a ordenação.

### Exercício 05 — Insertion Sort Decrescente

Implementação de uma variação do **Insertion Sort** para ordenação dos elementos em ordem decrescente.

## Requisitos

Para compilar e executar o projeto é necessário possuir:

* Compilador C++
* CMake compatível com a versão definida no `CMakeLists.txt`
* CLion ou outra IDE compatível com projetos CMake

## Compilação pelo terminal

Dentro da pasta raiz do projeto, execute:

```bash
cmake -S . -B build
```

Esse comando cria a pasta de compilação e gera os arquivos necessários.

Depois execute:

```bash
cmake --build build
```

O CMake irá compilar todos os executáveis definidos no projeto.

## Execução pelo CLion

1. Abra o CLion.
2. Selecione **File → Open**.
3. Abra a pasta raiz deste projeto.
4. Aguarde o carregamento do `CMakeLists.txt`.
5. No topo da IDE, selecione o exercício que deseja executar.

Exemplo:

```text
Exer01_BubbleSortString
```

6. Clique no botão **Run**.

Também é possível executar utilizando o atalho:

```text
Shift + F10
```

Para executar outro exercício, selecione o executável correspondente no topo do CLion.

## Testes

Cada exercício possui casos de teste responsáveis por comparar o resultado produzido pelo algoritmo com o resultado esperado.

Para executar os testes:

1. Abra o arquivo do exercício desejado.
2. Selecione o executável correspondente no CLion.
3. Clique em **Run** ou pressione `Shift + F10`.
4. Observe o resultado no console.

Exemplo de execução:

```text
Input:           patrocinio
Expected Output: aciinooprt
Actual Output:   aciinooprt
[PASSED]
```

Quando aparecer:

```text
[PASSED]
```

significa que o resultado produzido pelo algoritmo corresponde ao resultado esperado.

Caso apareça:

```text
[FAILED]
```

significa que o resultado obtido foi diferente do valor esperado pelo teste.

## Execução de todos os exercícios

Os seguintes executáveis estão disponíveis no projeto:

```text
Exer01_BubbleSortString
Exer02_SelectionSortDescending
Exer03_SelectionSortKSwaps
Exer04_InsertionSortShiftCount
Exer05_InsertionSortDescendingTail
```

Cada um pode ser compilado e executado separadamente pelo CLion.

## Organização da atividade

Esta atividade prática é composta por duas etapas.

A primeira etapa consiste na disponibilização do código-fonte completo e estruturado em um repositório no GitHub, incluindo este arquivo `README.md` com instruções para compilação, execução e testes.

A segunda etapa consiste na gravação de um vídeo demonstrativo apresentando:

* explicação do código-fonte;
* funcionamento dos algoritmos;
* execução dos exercícios;
* breve explicação sobre o processo de desenvolvimento da solução.

## Autor

**Lucas Carvalho**

Estudante de Análise e Desenvolvimento de Sistemas — IFTM
