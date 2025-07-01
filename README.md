# 🏋️‍♀️ Sistema de Academia - Trabalho Final POO (2025/1)

Este repositório contém a implementação do Trabalho Final da disciplina de Programação Orientada a Objetos (POO), ministrada pelo professor Daniel Callegari.

## 💡 Tema do Projeto

Sistema de gerenciamento de **academia**, permitindo o cadastro, controle de treino, e gerenciamento de funcionários e alunos. A aplicação conta com controle de liberação de acesso, estatísticas e interface gráfica com Java Swing.

## 🎯 Objetivos do Projeto

Este projeto tem como principais objetivos:

- Aplicar os conceitos de **herança** e **polimorfismo**
- Utilizar **programação orientada a eventos**
- Implementar **coleções** em memória e utilizar **programação funcional**
- Construir uma **interface gráfica com Java Swing**
- Desenvolver uma solução modular com boas práticas de codificação

## 🧱 Estrutura do Projeto

- **Interface Gráfica**:
  - Implementada com Java Swing
  - Janela principal (`Teste.java`)
  - Telas de visualização, cadastro, estatísticas e painel do caixa

- **Entidades e Hierarquia de Classes**:
  - `Pessoa` (superclasse)
    - `Aluno`
    - `Funcionario` (classe abstrata)
      - `FuncionarioCaixa`
      - `FuncionarioProfessor`
  - Outras classes:
    - `Academia` (classe de controle geral)
    - `Treino` e `Exercicio` (ligados aos alunos)

- **Coleções**:
  - Objetos armazenados em memória com `List<>`
  - Sem persistência em arquivos ou banco de dados

- **Estatísticas Exibidas**:
  - Total de cadastros e por tipo (Aluno, Funcionário)
  - Soma dos valores pagos pelos alunos
  - Média de idade dos alunos

- **Funcionalidade Extra**:
  - O **caixa** (representado pela classe `FuncionarioCaixa`) deve liberar o aluno antes que ele possa iniciar o treino.
  - Sem liberação, o aluno é impedido de treinar, garantindo controle de acesso.

## ✅ Funcionalidades Implementadas

- [x] Cadastro de alunos e funcionários
- [x] Busca por nome
- [x] Visualização de todos os cadastros
- [x] Painel de estatísticas (contagem, soma e média)
- [x] Controle de liberação pelo caixa antes do treino (funcionalidade extra)
- [x] Interface gráfica com botões, campos e ações interativas

## 🚫 Restrições Atendidas

- ❌ Não há uso de banco de dados nem arquivos para persistência
- ✅ Todos os dados residem somente em memória RAM durante a execução
- ✅ O sistema já inicia com dados de exemplo prontos para testes

## 🧪 Tecnologias e Conceitos Usados

- Java 17+
- Java Swing
- Programação Orientada a Objetos
- Classes abstratas, herança, polimorfismo
- Lambda Expressions e Stream API

## 👨‍🏫 Avaliação

| Critério                                 | Pontuação |
|------------------------------------------|-----------|
| Entidades de domínio bem definidas       | 2,5       |
| Interface gráfica funcional              | 2,5       |
| Funcionalidades requeridas completas     | 4,0       |
| Qualidade geral do código                | 1,0       |
| **Total**                                | **10,0**  |

## 🚀 Como Executar

1. Clone o repositório:
   ```bash
   git clone https://github.com/emivargxs/sistema-academia-poo.git
