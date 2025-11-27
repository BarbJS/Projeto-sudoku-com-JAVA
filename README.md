# 🧩 Projeto Sudoku com Java 

Um jogo de Sudoku completo e modular desenvolvido em Java, focado em demonstrar conceitos de Orientação a Objetos, Clean Code e uso eficiente da API de Streams do Java.

## 📋 Sobre o Projeto

Este projeto implementa a lógica do clássico jogo Sudoku rodando diretamente no terminal. Ele foi construído seguindo boas práticas de desenvolvimento de software, como encapsulamento, imutabilidade (onde aplicável) e separação de responsabilidades. O tabuleiro é gerado dinamicamente com base em argumentos passados na inicialização, permitindo diferentes configurações de jogo. Este projeto foi criado para cumprimento do Desafio - Criando um Jogo de Sudoku em Java, proposto e orientado pelo professor 
José Luiz Abreu Cardoso Junior, do curso de Formação Java Fundamentals, da plataforma de ensino DIO (Digital Innovation One).

## ✨ Principais Funcionalidades

* **Tabuleiro Interativo:** Visualização clara do tabuleiro no console.
* **Validação em Tempo Real:** Verificação de status do jogo (Não iniciado, Incompleto e Completo).
* **Detecção de Erros:** O sistema alerta se o usuário inseriu um número incorreto (com base na solução esperada).
* **Posições Fixas:** Respeito às regras do Sudoku onde números iniciais (fixos) não podem ser alterados.
* **Menu de Opções:** Interface amigável para inserir e remover números, limpar o jogo e verificar progresso.

## 🛠️ Tecnologias Utilizadas

* **Java 17+** (Uso de Records, Text Blocks, Switch Expressions e Streams).
* **Conceitos:** Enumerações, Mapas, Listas e Streams.

## 📂 Estrutura do Projeto

br.com.dio.Main: Classe principal que gerencia o loop do jogo.

br.com.dio.model.Board: Representa o tabuleiro e suas regras.

br.com.dio.model.Space: Representa cada célula do Sudoku.

br.com.dio.util.BoardTemplate: Utilitário para desenhar o tabuleiro.

## 🚀 Como Executar

Para rodar o jogo, é necessário passar a configuração do tabuleiro como argumentos de linha de comando (Program Arguments). A string de configuração define a posição, o valor esperado e se o número é fixo.

### Pré-requisitos
* JDK 11 ou superior instalado.

### Passos
1.  Clone ou baixe o repositório. Abra a pasta do projeto no seu editor de código.
2.  Execute a classe `Main` passando a seguinte string de argumentos:

```bash: 0,0;4,false 1,0;7,false 2,0;9,true 3,0;5,false 4,0;8,true 5,0;6,true 6,0;2,true 7,0;3,false 8,0;1,false 0,1;1,false 1,1;3,true 2,1;5,false 3,1;4,false 4,1;7,true 5,1;2,false 6,1;8,false 7,1;9,true 8,1;6,true 0,2;2,false 1,2;6,true 2,2;8,false 3,2;9,false 4,2;1,true 5,2;3,false 6,2;7,false 7,2;4,false 8,2;5,true 0,3;5,true 1,3;1,false 2,3;3,true 3,3;7,false 4,3;6,false 5,3;4,false 6,3;9,false 7,3;8,true 8,3;2,false 0,4;8,false 1,4;9,true 2,4;7,false 3,4;1,true 4,4;2,true 5,4;5,true 6,4;3,false 7,4;6,true 8,4;4,false 0,5;6,false 1,5;4,true 2,5;2,false 3,5;3,false 4,5;9,false 5,5;8,false 6,5;1,true 7,5;5,false 8,5;7,true 0,6;7,true 1,6;5,false 2,6;4,false 3,6;2,false 4,6;3,true 5,6;9,false 6,6;6,false 7,6;1,true 8,6;8,false 0,7;9,true 1,7;8,true 2,7;1,false 3,7;6,false 4,7;4,true 5,7;7,false 6,7;5,false 7,7;2,true 8,7;3,false 0,8;3,false 1,8;2,false 2,8;6,true 3,8;8,true 4,8;5,true 5,8;1,false 6,8;4,true 7,8;7,false 8,8;9,false```

### Observação: Se estiver usando uma IDE (IntelliJ ou Eclipse), adicione a string acima no campo "Program Arguments" nas configurações de execução.
