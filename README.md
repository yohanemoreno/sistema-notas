# Sistema de Notas v4.1

Este é um programa em **C++** desenvolvido para console (Windows) que gerencia o cadastro de alunos, a inserção de notas por disciplinas, o cálculo de médias e a classificação final de cada aluno (Aprovado, Recuperação ou Reprovado). O sistema também conta com funcionalidades para salvar os relatórios gerados em arquivos de texto e carregar relatórios salvos anteriormente.

---

## 🚀 Funcionalidades

- **Menu Inicial:** Permite escolher entre gerar um novo relatório ou abrir um relatório já existente.
- **Menu "Sobre meu sistema:** Da informações sobre o sistema, quem o desenvolveu, entre outras informações.
- **Cadastro de Alunos e Disciplinas:** Permite a inserção de dados dos alunos e suas notas por disciplina.
- **Validação de Entradas:** Garante que o número de alunos (1 a 20), o número de disciplinas (1 a 5) e as notas inseridas (1 a 10) estejam dentro dos limites permitidos.
- **Cálculo Automático:** Calcula a média aritmética de cada aluno com base no número de disciplinas configurado.
- **Classificação Estatística:**
  - **Média ≥ 7.0:** Aprovado
  - **Média entre 5.0 e 6.9:** Recuperação
  - **Média < 5.0:** Reprovado
- **Persistência de Dados:** Salva automaticamente o relatório final e o resumo estatístico em um arquivo chamado `relatorio.txt` salvo com data e hora.
- **Leitura de relatório salvo:** Recupera o arquivo relatorio.txt salvo no disco e exibe todo o seu histórico formatado diretamente no console do sistema. 


---

## 🛠️ Tecnologias Utilizadas

- **Linguagem:** C++
- **Biblioteca Padrão:** `<iostream>`, `<string>`, `<fstream>`
- **API do Windows:** `<windows.h>` (utilizada para a configuração de codificação do console para UTF-8 através da função `SetConsoleOutputCP(65001)`).

---

## 📁 Estrutura de Arquivos do Projeto

O ciclo de desenvolvimento do código foi documentado através de marcações de commits estruturados da seguinte forma:

- **Commit 1:** Implementação da leitura e validação dos dados dos alunos.
- **Commit 2:** Adição da lógica de captura de notas por disciplina e cálculo de médias.
- **Commit 3:** Criação da lógica de classificação (Aprovado/Recuperação/Reprovado), exibição do resumo estatístico 
- **Commit 4:** Integração do sistema de persistência para exportar dados no arquivo `relatorio.txt´. 
- **Commit 5:** Implementação da funcionalidade de leitura e exibição do arquivo gravado através do menu inicial.

---

## 💻 Como Executar o Projeto

### Pré-requisitos
Como o código utiliza a biblioteca `<windows.h>`, ele foi projetado especificamente para ambientes **Windows**. Você precisará de um compilador C++ (como o GCC/MinGW) ou de uma IDE como o Visual Studio, Code::Blocks ou Dev-C++.

### Passo a Passo

1. **Clone ou baixe o código fonte:**
   Salve o código em um arquivo chamado `main.cpp`.

2. **Compilação via Terminal (Prompt de Comando ou PowerShell):**
   ```bash
   g++ main.cpp -o SistemaNotas.exe