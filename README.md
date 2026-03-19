#  Projeto de Compiladores: Analisador C# com JavaCC

Este repositório contém a implementação de um analisador léxico e sintático desenvolvido como projeto para a disciplina de Compiladores. A ferramenta foi construída utilizando **JavaCC** (Java Compiler Compiler) e tem como objetivo reconhecer e validar as estruturas gramaticais da linguagem **C#**.

## 📋 Escopo do Projeto

O compilador foi desenhado para contemplar as seguintes estruturas da linguagem C#:
- Tipos básicos: `string`, números (inteiro e real).
- Atribuições de variáveis.
- Declaração e chamada de funções.
- Laço de repetição (`while` ou `for`).
- Estrutura condicional simples e composta (`if` / `else`).
- Comandos de entrada e saída (`Console.ReadLine` e `Console.WriteLine`).
- Expressões matemáticas e lógicas.
- Operadores relacionais, aritméticos e booleanos.

## 👥 Divisão da Equipe

O desenvolvimento do arquivo `.jj` foi dividido em 4 frentes principais:

1. **Analisador Léxico (Dicionário e Tokens):** Laryssa Finizola - *Concluído* ✅
2. **Analisador Sintático (Expressões e Atribuições):** [Nome do Colega 2] - *Em desenvolvimento* ⏳
3. **Analisador Sintático (Controle de Fluxo e I/O):** [Nome do Colega 3] - *Em desenvolvimento* ⏳
4. **Analisador Sintático (Funções e Escopo):** [Nome do Colega 4] - *Em desenvolvimento* ⏳

---

## 🔍 Evidência: Analisador Léxico em Ação

Nesta primeira etapa, o analisador léxico foi finalizado. Ele é capaz de ler um arquivo fonte em C# e extrair com sucesso todos os tokens, ignorando espaços em branco e validando palavras reservadas, variáveis e símbolos.

Abaixo, a demonstração da CLI (Command Line Interface) do Eclipse lendo o arquivo `teste.txt` contendo o código `int valor = 10;`:

> O programa identificou perfeitamente o tipo, o identificador, o operador de atribuição, o número inteiro e o delimitador de linha.


<img width="557" height="233" alt="analisador-lexico" src="https://github.com/user-attachments/assets/ea7a32be-a4b2-43d1-a5bf-daf0e7a2ee76" />

---

## 🛠️ Tecnologias e Pré-requisitos

Para rodar este projeto na sua máquina, você precisará de:
* **Java JDK 17** (ou superior)
* **Eclipse IDE** com o plugin **JavaCC** instalado (via Eclipse Marketplace)

## 🚀 Como Executar

1. Clone este repositório.
2. Importe o projeto no Eclipse.
3. Certifique-se de que o arquivo fonte a ser analisado se chama `teste.txt` e está localizado na raiz do projeto.
4. Caso faça alterações no arquivo `Compilador.jj`, salve-o para que o plugin do JavaCC regenere os arquivos `.java`.
5. Execute o arquivo `Compilador.java` como uma Aplicação Java (Run As > Java Application).
6. O resultado da análise (tokens encontrados ou erros de sintaxe) será exibido no console.
