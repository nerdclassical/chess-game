♟️ Java Chess System
Um sistema de xadrez completo via console, desenvolvido para aplicar conceitos avançados de Programação Orientada a Objetos e Arquitetura de Software.

O projeto separa rigidamente a lógica de estrutura de dados (tabuleiro) da lógica de regras de negócio (xadrez), demonstrando domínio sobre encapsulamento, herança, polimorfismo e tratamento de exceções.

📋 Índice
Sobre o Projeto

Arquitetura e Design

Funcionalidades

Tecnologias Utilizadas

Como Executar

📖 Sobre o Projeto
Este projeto consiste em um jogo de xadrez jogável via terminal. O objetivo principal não é apenas criar um jogo, mas construir uma aplicação sustentável e extensível. O sistema é capaz de:

Validar movimentos baseados nas regras oficiais do xadrez.

Gerenciar turnos e captura de peças.

Identificar estados de jogo complexos como Xeque e Xeque-Mate.

Lidar com movimentos especiais (Roque, En Passant, Promoção).

🏗 Arquitetura e Design
O sistema foi projetado seguindo o padrão de Camadas (Layered Architecture) para garantir o desacoplamento:

1. Board Layer (Camada de Tabuleiro)
A camada de "baixo nível". Ela é agnóstica às regras do xadrez.

Responsabilidade: Gerenciar a matriz de peças, verificar limites do tabuleiro e alocar posições.

Conceitos: Matrizes, Tratamento de Exceções Personalizadas (BoardException).

2. Chess Layer (Camada de Xadrez)
A camada de "regras de negócio". Ela consome a camada de tabuleiro.

Responsabilidade: Validar movimentos de peças específicas (Torre, Rei, Bispo, etc.), gerenciar turnos, verificar xeque/xeque-mate.

Conceitos: Herança, Polimorfismo, Sobrescrita de Métodos.

3. Application Layer (Aplicação)
A camada de interação.

Responsabilidade: Interagir com o usuário via terminal, processar inputs e renderizar o estado atual da partida.

🚀 Funcionalidades
[x] Tabuleiro e Impressão no Console

[x] Movimentos Básicos de Peças

[x] Validação de Movimentos Possíveis

[x] Lógica de Xeque e Xeque-Mate

[x] Movimentos Especiais:

[x] Roque (Castling)

[x] En Passant

[x] Promoção de Peão
