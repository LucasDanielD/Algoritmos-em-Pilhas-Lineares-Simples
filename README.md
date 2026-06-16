# Algoritmos-em-Pilhas-Lineares-Simples
# 📚 Estruturas de Dados: Algoritmos em Filas (Queues)

> **Disciplina:** Estrutura de Dados I  
> **Linguagem:** Java ☕  
> **Conceitos abordados:** Filas (Estáticas e Dinâmicas), Pilhas (Stacks), Herança, Manipulação de Ponteiros e Orientação a Objetos.

Este repositório contém a resolução de uma bateria de exercícios práticos focados na estrutura de dados **Fila (Queue)**. O projeto explora implementações baseadas em vetores lineares (abordagem estática) e nós encadeados (abordagem dinâmica), além de operações complexas de mesclagem, contagem e simulação.

---

## 🚀 O que foi desenvolvido?

O projeto está dividido em seis exercícios principais, cada um focado em um aspecto avançado da manipulação de filas:

### 🧱 Bloco A: Abordagens Estáticas (Vetores)

* ✅ **[Exer01] Deslocamento Imediato (`Exer01ShiftPop`)** Implementação do método `pop()` em uma fila estática. Ao remover o primeiro elemento (índice 0), o algoritmo realiza o deslocamento imediato (shift) de todos os itens restantes para a esquerda, garantindo que a frente da fila esteja sempre na base do vetor. Feito com base no reuso de código via herança da `ArrayQueue`.

* ✅ **[Exer02] Fila Utilizando Duas Pilhas (`Exer02StackBasedQueue`)** Simulação do comportamento de uma Fila (FIFO - *First In, First Out*) utilizando como "motor" interno exclusivamente duas estruturas do tipo Pilha (LIFO - *Last In, First Out*). Nenhuma estrutura de array nativo foi utilizada nesta implementação, apenas a lógica de transferência de estado entre as pilhas de entrada e saída.

* ✅ **[Exer03] Fila com Saída Dupla (`Exer03OutputRestrictedDeque`)** Implementação de um *Output-Restricted Deque*. Uma evolução da fila convencional que permite remover elementos tanto do início (comportamento padrão) quanto do final da estrutura através do método customizado `popBack()`.

### 🧬 Bloco B: Abordagens Dinâmicas (Nós Encadeados)

* ✅ **[Exer04] Contagem com Estrutura Preservada (`Exer04CountOccurrences`)** Algoritmo de busca e contagem de ocorrências de um valor específico (`target`) em uma Fila Dinâmica. A restrição rigorosa de utilizar apenas os métodos públicos `push` e `pop` foi respeitada através do uso de uma fila auxiliar, garantindo que ao final do processo a estrutura original retornasse à sua exata ordem de entrada.

* ✅ **[Exer05] Junção de Filas Ordenadas / *Merge* (`Exer05MergeQueues`)** Algoritmo clássico de *Merge*. Recebe duas filas dinâmicas já ordenadas de forma crescente e as combina em uma terceira fila resultante, mantendo a ordenação perfeita e esvaziando as filas de origem no processo.

* ✅ **[Exer06] Separação Par e Ímpar (`Exer06SplitEvenOdd`)** Procedimento que consome uma fila dinâmica original e distribui seus elementos em duas novas filas (uma contendo exclusivamente pares e outra contendo ímpares). O algoritmo preserva estritamente a ordem cronológica de chegada dos dados originais.

---

## 📂 Estrutura do Projeto

O projeto baseia-se na implementação de interfaces fundamentais (`Queue<T>` e `Stack<T>`).

```text
📦 src/main/java/dev/junio
 ┣ 📂 queue
 ┃ ┣ 📂 arrayqueue     # Fila baseada em vetor de tamanho fixo
 ┃ ┣ 📂 linkedqueue    # Fila dinâmica baseada em nós encadeados
 ┃ ┣ 📂 exercises      # Classes com a resolução dos 6 exercícios
 ┃ ┗ 📜 Queue.java     # Interface de Contrato da Fila
 ┗ 📂 stack
   ┣ 📂 arraystack     # Pilha baseada em vetor
   ┣ 📂 linkedstack    # Pilha baseada em nós encadeados
   ┗ 📜 Stack.java     # Interface de Contrato da Pilha
