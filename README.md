# Sistema de Gestão Acadêmica (Controle de Notas e Frequência)

Um sistema completo em Python desenvolvido para cadastro, validação de dados acadêmicos, cálculo de médias e geração de boletim consolidado por estudante.

---

## Sumário
- [Sobre o Projeto](#-sobre-o-projeto)
- [Funcionalidades](#-funcionalidades)
- [Regras de Negócio](#-regras-de-negócio)
- [Tecnologias Utilizadas](#-tecnologias-utilizadas)
- [Estrutura do Repositório](#-estrutura-do-repositório)
- [Como Executar o Projeto](#-como-executar-o-projeto)
- [Autor](#-autor)

---

## Sobre o Projeto

O **Sistema de Gestão Acadêmica** permite cadastrar estudantes e registrar notas e presença em disciplinas padronizadas (*Matemática, Português, Ciências, História e Geografia*). O programa valida todas as entradas de dados do usuário e gera um relatório final completo com status de aprovação, verificação de dependências e taxa de frequência global.

---

## Funcionalidades

- Cadastro Inteligente de Alunos: Registro de múltiplos estudantes com encerramento dinâmico (`sair`).
- Validação Rígida de Entradas.
- Notas restritas ao intervalo de **0 a 10**.
- Frequência restrita ao intervalo de **0 a 100%**.
- Tratamento de exceções para entradas não numéricas (`ValueError`).
- Cálculo Automático.
- Média aritmética por disciplina.
- Média geral do semestre.
- Frequência global do estudante.
- Relatório Final Estruturado: Exibição em formato de boletim acadêmico detalhado por matéria e status global final.

---

## Regras de Negócio

### Por Disciplina:
- **Média ≥ 6.0**: Aprovado
- **4.0 ≤ Média < 6.0**: Recuperação
- **Média < 4.0**: Reprovado por Nota

### Status Final do Aluno:
- **Frequência Global < 75.0%**: Reprovado por Frequência
- **Frequência ≥ 75.0% com matérias abaixo de 6.0**: Atenção - Aluno em Recuperação ou Reprovado em disciplinas
- **Frequência ≥ 75.0% e Aprovado em todas as matérias**: Aprovado com Sucesso!

---

##  Tecnologias Utilizadas

- **Python 3.x** (estruturas de dados, funções modularizadas e tratamento de exceções)

---
controle-notas-python/
│-- main.py          # Código principal da aplicação
│-- README.md        # Documentação detalhada do projeto
