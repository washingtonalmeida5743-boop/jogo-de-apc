# WMLETRAS - Jogo de Palavras Cruzadas

**Autor:** Washington Matheus Almeida Xavier  
**Disciplina:** Algoritmos e Programação de Computadores (APC)

## 🎮 Sobre o Projeto

**WMLETRAS** é um jogo de lógica e vocabulário desenvolvido em linguagem C. O objetivo é formar palavras a partir de um conjunto de letras embaralhadas. O jogo possui um sistema de progressão de níveis, pontuação dinâmica e um ranking persistente que salva o histórico dos melhores jogadores.

O projeto foi desenvolvido com foco na manipulação de arquivos (leitura de fases e escrita de ranking binário), alocação de memória e construção de interfaces interativas via terminal.

## 🚀 Funcionalidades

* **Sistema de Menus Interativo:** Navegação controlada pelo teclado (não requer mouse).
* **Leitura de Arquivos:** As fases são carregadas externamente via `entrada.txt`, permitindo a criação de novos níveis sem recompilar o código.
* **Ranking Persistente:** Os recordes são salvos em um arquivo binário (`ranking.bin`), mantendo os dados mesmo após fechar o jogo.
* **Estilização Visual:** Uso de códigos ANSI para cores e limpeza de tela, proporcionando uma interface estilo "Matrix/Hacker".
* **Easter Eggs:** Códigos secretos escondidos nas configurações.

## 🛠️ Como Compilar e Executar

### Pré-requisitos
* Compilador C (GCC/MinGW).
* Sistema Operacional Windows (recomendado devido ao uso de bibliotecas de sistema) ou Linux.

### Passo a Passo

1.  Compile o código fonte:
    ```bash
    gcc 252024622.c.c -o wmletras.exe
    ```

2.  **Importante:** Certifique-se de que o arquivo `entrada.txt` esteja na **mesma pasta** do executável (`wmletras.exe`).

3.  Execute o jogo:
    ```bash
    ./wmletras.exe
    ```

## 🕹️ Como Jogar

### Controles do Menu
* `W`: Mover para cima.
* `S`: Mover para baixo.
* `F`: Confirmar seleção/Entrar.

### Regras do Jogo
1.  O jogo apresentará um conjunto de letras embaralhadas (ex: `A R O M`).
2.  Você deve digitar palavras que podem ser formadas com essas letras (ex: `AMOR`, `ROMA`).
3.  **Pontuação:**
    * Acerto: +100 pontos.
    * Erro: -10 pontos.
    * Passar de Fase: +25 pontos.
4.  Para salvar e sair durante o jogo, digite `SAIR`.

## 📂 Estrutura dos Arquivos

* `252024622.c.c`: Código fonte principal do jogo.
* `entrada.txt`: Arquivo de texto contendo as fases (Letras embaralhadas e respostas).
* `ranking.bin`: Arquivo binário gerado automaticamente para salvar os recordes.

## ⚙️ Configuração Personalizada

Você pode editar o arquivo `entrada.txt` para adicionar suas próprias fases seguindo este padrão:
```text
LETRAS_EMBARALHADAS
NUMERO_DE_RESPOSTAS
RESPOSTA1 RESPOSTA2 RESPOSTA3...
-
