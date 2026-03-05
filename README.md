#Atividade Avaliativa


## 🔹 Questão 1

O HeapSort possui complexidade garantida de O(n log n) em todos os casos porque utiliza uma estrutura de Heap (árvore binária completa).

A construção do heap possui custo O(n).  
Cada uma das n remoções da raiz possui custo O(log n), pois a altura da árvore é proporcional a log n.

Logo, o custo total do algoritmo é:

T(n) = n log n

Como a altura da árvore é sempre log n, o tempo de execução é previsível tanto no melhor, médio e pior caso.

Já o ShellSort não possui complexidade garantida, pois depende da sequência de gaps utilizada. Dependendo da sequência escolhida, sua complexidade pode variar entre aproximadamente O(n log² n) e O(n²). Portanto, não há garantia formal de desempenho fixo.

---

## 🔹 Questão 2

Vetor dado:

[30, 12, 45, 6, 18, 3]

### a) Max-Heap correspondente

Após aplicar o processo de heapify, o Max-Heap é:

[45, 18, 30, 6, 12, 3]

Representação em árvore:

        45
       /  \
     18    30
    /  \    /
   6   12   3

### b) Vetor após a primeira extração da raiz

1. Remove-se o elemento 45.
2. O último elemento (3) é colocado na raiz.
3. Aplica-se heapify para reorganização.

Resultado:

[30, 18, 3, 6, 12]

---

## 🔹 Questão 3

Análise das afirmativas:

I – ShellSort é estável.  
Falsa. O ShellSort não é estável.

II – HeapSort utiliza estrutura baseada em árvore binária completa.  
Verdadeira.

III – HeapSort depende da sequência de gaps.  
Falsa. Quem depende de gaps é o ShellSort.

IV – ShellSort é uma melhoria do Insertion Sort.  
Verdadeira.

Alternativa correta:

A) Apenas II e IV

---

## 🔹 Questão 4

Para um sistema que processa milhões de registros diariamente, o algoritmo mais indicado é o HeapSort.

Justificativa:

- Complexidade garantida O(n log n)
- Desempenho previsível
- Não depende da ordem inicial dos dados
- Não degrada para O(n²)

Em sistemas de grande escala, previsibilidade é essencial.

---

## 🔹 Questão 5

A estrutura Heap é utilizada como fila de prioridade em algoritmos de grafos.

Ela permite:

- Inserção em O(log n)
- Remoção do menor elemento em O(log n)

Um exemplo clássico é o algoritmo de Dijkstra, onde o heap é utilizado para selecionar o vértice com menor distância acumulada ainda não processado.

Com o uso de Heap (Min-Heap), a complexidade do algoritmo torna-se:

O((V + E) log V)

Sem heap, o desempenho seria inferior.

---

# 📌 Conclusão

O HeapSort apresenta maior previsibilidade e garantia de desempenho, sendo mais indicado para aplicações de grande escala.  
O ShellSort, apesar de eficiente em alguns casos práticos, não possui limite superior fixo de complexidade.
