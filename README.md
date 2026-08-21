# ED2 — Sorting — Lista 01

Projeto desenvolvido para a disciplina de **Estrutura de Dados II**, com foco na implementação e prática de algoritmos clássicos de ordenação em C++.

A lista trabalha com variações dos algoritmos:

* Bubble Sort
* Selection Sort
* Insertion Sort

## Tecnologias utilizadas

* C++
* CMake
* CLion
* Git

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

Cada exercício possui seu próprio arquivo `.cpp` e pode ser compilado e executado separadamente.

## Exercícios

### Exercício 01 — Bubble Sort em String

Utiliza o algoritmo **Bubble Sort** para ordenar os caracteres de uma string em ordem crescente.

Exemplo:

```text
Entrada:
patrocinio

Saída:
aciinooprt
```

### Exercício 02 — Selection Sort Decrescente

Implementação do **Selection Sort** para ordenar os elementos em ordem decrescente.

### Exercício 03 — Selection Sort com K trocas

Variação do **Selection Sort** considerando uma quantidade limitada de trocas.

### Exercício 04 — Insertion Sort e deslocamentos

Implementação do **Insertion Sort**, contabilizando os deslocamentos realizados durante o processo de ordenação.

### Exercício 05 — Insertion Sort Decrescente

Variação do **Insertion Sort** para realizar a ordenação em ordem decrescente.

## Compilação

O projeto utiliza **CMake**.

Dentro da pasta do projeto:

```bash
cmake -S . -B build
cmake --build build
```

Também é possível abrir diretamente o projeto no **CLion**, que reconhece automaticamente o arquivo `CMakeLists.txt`.

## Execução no CLion

No CLion, selecione no topo o exercício que deseja executar, por exemplo:

```text
Exer01_BubbleSortString
```

Em seguida, clique em **Run** ou utilize:

```text
Shift + F10
```

Cada exercício é executado independentemente.

## Objetivo

O objetivo deste projeto é praticar o funcionamento dos algoritmos de ordenação elementares e compreender aspectos como:

* comparação entre elementos;
* realização de trocas;
* deslocamento de valores;
* ordenação crescente e decrescente;
* comportamento dos algoritmos em diferentes situações.

## Autor

**Lucas Carvalho**

Estudante de Análise e Desenvolvimento de Sistemas — IFTM
