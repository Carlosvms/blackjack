# Blackjack(21) em Java

Projeto desenvolvido para a disciplina da faculdade, implementando o clássico jogo de cartas **Blackjack (21)** em linguagem Java com interface via terminal/console.

## Sobre o Projeto

O jogo simula uma partida entre um jogador humano e a máquina (dealer), utilizando estruturas de dados como pilha customizada e listas para o gerenciamento do baralho e das mãos de cartas.

### Funcionalidades
- **Baralho completo**: 52 cartas com naipes (copas, ouros, espadas, paus) e valores de Ás a Rei.
- **Estruturas de Dados**: Implementação de Pilha encadeada dinâmica para o baralho (nós e referências).
- **Lógica de Blackjack**:
  - Tratamento dinâmico do valor do Ás (1 ou 11).
  - Cálculo de pontuação e verificação de estouro (> 21).
  - Carta oculta da máquina durante o turno inicial.
  - Regras de parada e compra para o jogador e estratégia automática para a máquina.
- **Visualização das cartas**: Exibição gráfica simplificada no terminal com naipes e bordas.

## Estrutura de Pastas

```
Blackjack/
├── src/
│   ├── Baralho/
│   │   ├── Carta.java
│   │   ├── Mao.java
│   │   ├── No.java
│   │   ├── Pilha.java
│   │   └── TestePilha.java
│   ├── Players/
│   │   ├── Jogador.java
│   │   ├── JogadorHumano.java
│   │   └── JogadorMaquina.java
│   └── Principal/
│       ├── Jogo.java
│       └── Main.java
├── .gitignore
└── README.md
```

## Como Executar

### Pré-requisitos
- JDK 17 ou superior instalado.

### Executando pelo Terminal
1. Compile os arquivos Java:
   ```bash
   javac -d out/production/Blackjack src/Baralho/*.java src/Players/*.java src/Principal/*.java
   ```
2. Execute o jogo:
   ```bash
   java -cp out/production/Blackjack Principal.Main
   ```

### Executando em uma IDE (IntelliJ IDEA / VS Code / Eclipse)
1. Abra a pasta do projeto na sua IDE favorita.
2. Execute a classe principal `src/Principal/Main.java`.
