# 🏦 Sistema Bancário em Python

Este projeto é um sistema bancário simples desenvolvido em Python, com funcionalidades básicas de **depósito**, **saque** e **extrato**. É uma aplicação de terminal que simula operações bancárias com algumas regras de negócio implementadas.

## 🚀 Funcionalidades

- **Depósito**
  - Permite adicionar um valor positivo à conta.
  - Atualiza o saldo e registra no extrato.

- **Saque**
  - Permite realizar saques com as seguintes regras:
    - Limite diário de **3 saques**.
    - Valor máximo por saque: **R$ 5000.00**.
    - Após as **18:00**, saques são limitados a **R$ 1000.00**.
    - O valor do saque não pode exceder o saldo disponível.
  - Atualiza o saldo e registra no extrato.

- **Extrato**
  - Exibe todas as transações realizadas.
  - Mostra o saldo atual e a quantidade de saques feitos.

- **Sair**
  - Encerra o programa.

## 🧠 Regras de Negócio

- Cada operação verifica se os valores inseridos são válidos.
- As tentativas inválidas são tratadas com mensagens informativas ao usuário.
- A lógica de horário usa a hora atual para restringir saques noturnos.

## 🛠️ Como usar

1. Certifique-se de ter o **Python 3.10+** instalado.
2. Clone o repositório:
   ```bash
   git clone https://github.com/GabrielSilvaG/Sistema.Bancario.DIO.git




📝 Exemplo de Uso

[d] Depositar
[s] Sacar
[e] Extrato
[q] Sair

=> d
Informe o valor do depósito: 1000

=> s
Informe o valor do saque: 200

=> e
================ EXTRATO ================
Depósito: R$ 1000.000
Saque: R$ 200.00

Saldo: R$ 800.00
Saques restantes: 1 / 3
==========================================


