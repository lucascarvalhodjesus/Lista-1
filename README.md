# ED2 — Algoritmos de Ordenação — Lista 01

Este repositório contém a resolução da **Lista 01 da disciplina de Estrutura de Dados II**, com exercícios relacionados a algoritmos elementares de ordenação.

O projeto foi desenvolvido em **C++** e utiliza **CMake** para compilação e organização dos executáveis.

## Objetivo

A atividade tem como objetivo praticar a implementação e compreensão de algoritmos clássicos de ordenação, trabalhando conceitos como:

* Bubble Sort;
* Selection Sort;
* Insertion Sort;
* ordenação crescente e decrescente;
* contagem de deslocamentos;
* limitação da quantidade de trocas;
* ordenação de strings;
* manipulação de vetores em C++.

## Tecnologias utilizadas

* C++
* CMake
* CLion
* Git
* GitHub

## Estrutura do projeto

```text
Lista-1-master/
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

Cada exercício possui seu próprio arquivo `.cpp` e seu próprio executável configurado no `CMakeLists.txt`.

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

O algoritmo compara caracteres vizinhos e realiza trocas quando o caractere da esquerda é maior que o da direita.

Também foi utilizada a variável `swapped` para interromper o algoritmo quando nenhuma troca for realizada, indicando que a string já está ordenada.

---

### Exercício 02 — Selection Sort Decrescente

Implementação do algoritmo **Selection Sort** para ordenar um vetor de números inteiros em ordem decrescente.

Exemplo:

```text
Entrada:
3 1 4 5 2

Saída:
5 4 3 2 1
```

A cada passagem, o algoritmo procura o maior elemento da parte ainda não ordenada do vetor e o coloca na posição correta.

---

### Exercício 03 — Selection Sort com K trocas

Implementação de uma variação do **Selection Sort** que executa somente uma quantidade determinada de etapas de ordenação.

Exemplo:

```text
Vetor:
29 64 14 37 13

k:
2
```

O algoritmo realiza somente as etapas determinadas pelo valor de `k`.

---

### Exercício 04 — Insertion Sort com contagem de deslocamentos

Implementação do algoritmo **Insertion Sort** em ordem crescente.

Durante a ordenação também é contabilizada a quantidade de deslocamentos realizados dentro do processo.

Exemplo utilizado:

```text
72 12 62 69 27 67 41 56 33 74
```

Vetor ordenado:

```text
12 27 33 41 56 62 67 69 72 74
```

A função retorna um `pair`, contendo:

```text
vector<int> → vetor ordenado
int         → quantidade de deslocamentos
```

---

### Exercício 05 — Insertion Sort Decrescente

Implementação de uma ordenação em ordem decrescente sobre um vetor de números inteiros.

Exemplo:

```text
Entrada:
12 7 9 15 3 1

Saída:
15 12 9 7 3 1
```

## Requisitos

Para compilar e executar o projeto é necessário possuir:

* compilador compatível com C++20;
* CMake;
* CLion ou outra IDE compatível com CMake.

O projeto utiliza:

```cmake
set(CMAKE_CXX_STANDARD 20)
```

## Compilação pelo terminal

Abra o terminal na pasta raiz do projeto.

Crie a pasta de build:

```bash
cmake -S . -B build
```

Depois compile o projeto:

```bash
cmake --build build
```

O CMake irá gerar os executáveis correspondentes a cada exercício.

## Executando pelo terminal

Após a compilação, os exercícios podem ser executados individualmente.

### Exercício 01

```bash
./build/Exer01_BubbleSortString
```

### Exercício 02

```bash
./build/Exer02_SelectionSortDescending
```

### Exercício 03

```bash
./build/Exer03_SelectionSortKSwaps
```

### Exercício 04

```bash
./build/Exer04_InsertionSortShiftCount
```

### Exercício 05

```bash
./build/Exer05_InsertionSortDescendingTail
```

## Executando pelo CLion

1. Abra o **CLion**.
2. Clique em **File → Open**.
3. Selecione a pasta raiz do projeto.
4. Aguarde o CLion carregar o arquivo `CMakeLists.txt`.
5. No canto superior direito, selecione o executável desejado.

Exemplo:

```text
Exer02_SelectionSortDescending
```

6. Clique no botão **Run ▶**.

Também é possível utilizar:

```text
Shift + F10
```

É importante selecionar o exercício correto antes de executar, pois cada arquivo possui seu próprio `main()`.

## Executáveis disponíveis

O `CMakeLists.txt` possui os seguintes executáveis:

```text
Exer01_BubbleSortString
Exer02_SelectionSortDescending
Exer03_SelectionSortKSwaps
Exer04_InsertionSortShiftCount
Exer05_InsertionSortDescendingTail
main_app
```

Cada exercício pode ser executado independentemente.

## Testes

Os arquivos possuem testes locais definidos pela função:

```cpp
runLocalTests();
```

Os testes comparam o resultado produzido pelo algoritmo com o resultado esperado.

Exemplo:

```text
Input:           3 1 4 5 2
Expected Output: 5 4 3 2 1
Actual Output:   5 4 3 2 1
[PASSED]
```

Quando aparece:

```text
[PASSED]
```

significa que o resultado produzido pelo algoritmo corresponde ao resultado esperado pelo teste.

Quando aparece:

```text
[FAILED]
```

significa que existe alguma diferença entre o resultado esperado e o resultado produzido pelo algoritmo.

## Organização do código

Os exercícios seguem uma estrutura semelhante:

```cpp
// implementação do algoritmo

// função para entrada do Online Judge

// testes locais

// função main
```

Durante o desenvolvimento, os testes locais são executados através de:

```cpp
runLocalTests();
```

A função `onlineJudge()` está disponível para adaptação caso seja necessário utilizar entrada pelo terminal ou por um sistema automático de correção.

## Finalidade acadêmica

Este projeto foi desenvolvido como parte de uma atividade prática da disciplina de **Estrutura de Dados II**.

O repositório contém:

* código-fonte completo;
* organização dos exercícios;
* configuração com CMake;
* testes locais;
* instruções para compilação;
* instruções para execução;
* instruções para testes.

## Autor

**Lucas Carvalho**

Estudante de Análise e Desenvolvimento de Sistemas — IFTM
