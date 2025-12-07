# ♟️ Java Chess System

![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![Git](https://img.shields.io/badge/GIT-E44C30?style=for-the-badge&logo=git&logoColor=white)

Um sistema de xadrez completo via console, desenvolvido para aplicar conceitos avançados de **Programação Orientada a Objetos** e **Arquitetura de Software**.

O projeto separa rigidamente a lógica de estrutura de dados (tabuleiro) da lógica de regras de negócio (xadrez), demonstrando domínio sobre encapsulamento, herança, polimorfismo e tratamento de exceções.

## 📋 Índice

- [Sobre o Projeto](#-sobre-o-projeto)
- [Arquitetura e Design](#-arquitetura-e-design)
- [Funcionalidades](#-funcionalidades)
- [Tecnologias Utilizadas](#-tecnologias-utilizadas)
- [Como Executar](#-como-executar)

---

## 📖 Sobre o Projeto

Este projeto consiste em um jogo de xadrez jogável via terminal. O objetivo principal não é apenas criar um jogo, mas construir uma aplicação sustentável e extensível. O sistema é capaz de:
- Validar movimentos baseados nas regras oficiais do xadrez.
- Gerenciar turnos e captura de peças.
- Identificar estados de jogo complexos como Xeque e Xeque-Mate.
- Lidar com movimentos especiais (Roque, En Passant, Promoção).

---

## 🏗 Arquitetura e Design

O sistema foi projetado seguindo o padrão de **Camadas (Layered Architecture)** para garantir o desacoplamento:

### 1. Board Layer (Camada de Tabuleiro)
A camada de "baixo nível". Ela é agnóstica às regras do xadrez.
- **Responsabilidade:** Gerenciar a matriz de peças, verificar limites do tabuleiro e alocar posições.
- **Conceitos:** Matrizes, Tratamento de Exceções Personalizadas (`BoardException`).

### 2. Chess Layer (Camada de Xadrez)
A camada de "regras de negócio". Ela consome a camada de tabuleiro.
- **Responsabilidade:** Validar movimentos de peças específicas (Torre, Rei, Bispo, etc.), gerenciar turnos, verificar xeque/xeque-mate.
- **Conceitos:** Herança, Polimorfismo, Sobrescrita de Métodos.

### 3. Application Layer (Aplicação)
A camada de interação.
- **Responsabilidade:** Interagir com o usuário via terminal, processar inputs e renderizar o estado atual da partida.

---

## 🚀 Funcionalidades

- [x] Tabuleiro e Impressão no Console
- [x] Movimentos Básicos de Peças
- [ ] Validação de Movimentos Possíveis
- [ ] Lógica de Xeque e Xeque-Mate
- [ ] Movimentos Especiais:
    - [ ] Roque (Castling)
    - [ ] En Passant
    - [ ] Promoção de Peão

---

## 💻 Tecnologias Utilizadas

- **Java 17+**: Linguagem core do sistema.
- **Programação Orientada a Objetos**:
    - Encapsulamento (proteção da matriz de peças).
    - Herança (`ChessPiece` estende `Piece`).
    - Polimorfismo (Movimentos variados por tipo de peça).
- **Git/GitHub**: Controle de versão.

---

## ⚡ Como Executar

### Pré-requisitos
Certifique-se de ter o [Java JDK](https://www.oracle.com/java/technologies/downloads/) instalado em sua máquina.

### Passo a passo

1. **Clone o repositório:**
   ```bash
   git clone [https://github.com/SEU-USUARIO/SEU-REPOSITORIO.git](https://github.com/SEU-USUARIO/SEU-REPOSITORIO.git)
