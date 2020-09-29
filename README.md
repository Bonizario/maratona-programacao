# :books: Maratona de Programação - 2020 - 1ª Fase (Intermediário)

### :chart_with_upwards_trend: Algoritmos de Ordenação

- Introdução
  - Bubble Sort, Merge Sort, Selection Sort, Insertion Sort, Quick Sort, etc
    - https://www.geeksforgeeks.org/sorting-algorithms
  - Animações/Explicações de cada algoritmo com pseudocódigo
    - https://www.toptal.com/developers/sorting-algorithms
  - Animações interativas
    - https://www.cs.usfca.edu/~galles/visualization/ComparisonSort.html

- Python 3
  - Exemplos em português (documentação oficial)
    - https://docs.python.org/pt-br/dev/howto/sorting.html
  - Diferença entre ```sort()``` e ```sorted()```:
    - ```list.sort()``` é um método de ordenação **estável** que modifica uma lista
    - ```sorted()``` retorna uma lista ordenada a partir de um iterável
  - Parâmetros das funções de ordenação: ```key``` e ```reverse```
  - Biblioteca **operator**: ```itemgetter()``` e ```attrgetter()```. Ordenação extremamente rápida de dicionários, classes, tuplas, etc.
    - https://docs.python.org/pt-br/dev/library/operator.html

###  Exercício 1548 - Fila do Recreio
```py3
n = int(input())

for _ in range(n):
    m = int(input())

    students = list(map(int, input().split()))
    ordered = sorted(students, reverse=True)

    not_changed = 0
    for i in range(m):
        if students[i] == ordered[i]:
            not_changed += 1

    print(not_changed)
```
