# Simulador de Movimentação de Xadrez ♟️

Este projeto em C simula o deslocamento de diferentes peças de xadrez em um tabuleiro virtual. O objetivo principal é demonstrar a aplicação de diversas estruturas de repetição e lógica de programação.

---

## 📋 Descrição do Código
O programa oferece um menu interativo onde o usuário escolhe uma peça e define a quantidade de casas que ela deve percorrer. Cada peça utiliza um método de repetição diferente para imprimir os movimentos no console:

* **Torre (♜):** Utiliza **Recursividade** para repetir o movimento para a direita.
* **Bispo (♝):** Utiliza o laço **`for`** para o movimento diagonal (Cima + Direita).
* **Rainha (♛):** Utiliza o laço **`while`** para o movimento para a esquerda.
* **Cavalo (♞):** Utiliza uma combinação de **`do-while`**, **`for`** e **recursividade** para simular o movimento em "L".

---

## ✨ Funcionalidades
* **Menu Interativo:** Um sistema robusto de `do-while` e `switch-case` para navegação.
* **Diversidade de Laços:** Demonstração técnica de todas as principais estruturas de controle de fluxo em C.
* **Entrada Dinâmica:** O usuário decide a distância (casas) que cada peça irá percorrer.

---

## 🛠️ Tecnologias Utilizadas
| Estrutura | Aplicação no Código |
| :--- | :--- |
| **Recursividade** | Funções `torre()` e `cavalo()` |
| **Laço `for`** | Função `bispo()` e parte da lógica do `cavalo()` |
| **Laço `while`** | Função `rainha()` |
| **Laço `do-while`** | Menu principal e parte da lógica do `cavalo()` |

---

## 🚀 Como Funciona a Lógica das Peças

### 1. Torre e Rainha
Movimentos lineares simples. Enquanto a torre "chama a si mesma" diminuindo o contador de casas, a rainha incrementa um contador até atingir o limite estipulado.

### 2. Bispo
Representa o movimento diagonal imprimindo dois eixos simultaneamente (`Cima, Direita`) a cada iteração do laço.

### 3. Cavalo
O movimento mais complexo:
* Executa um `do-while` interno para subir 2 casas (**Cima ↑**).
* Executa um `for` para mover 1 casa lateral (**Direita →**).
* Repete o processo via recursividade baseada no número de movimentos solicitados.

---

## 📄 Exemplo de Saída
```text
Escolha qual peça você quer mexer: 
[1] TORRE 
...
Digite quantas vezes você andará( ♜ ♖ ): 3
Direita → Direita → Direita →
