# Sistema Bancário Orientado a Objetos

## Descrição do Projeto

Este projeto consiste na implementação de um **sistema bancário em Python**, utilizando os conceitos de **Programação Orientada a Objetos (POO)**.

O objetivo principal é substituir estruturas simples como **dicionários** por **classes e objetos**, seguindo um modelo baseado em **diagrama UML**, garantindo maior organização, reutilização de código e escalabilidade.

O sistema permite o gerenciamento de:

* Clientes
* Contas bancárias
* Transações (depósito e saque)
* Histórico de movimentações

---

## Objetivos

* Aplicar conceitos de POO:

  * Encapsulamento
  * Herança
  * Abstração
  * Polimorfismo
* Implementar um sistema bancário funcional
* Utilizar classes no lugar de estruturas simples
* Seguir um modelo UML proposto

---

## Estrutura do Sistema

O sistema é dividido nas seguintes classes:

### Cliente

Responsável por representar um cliente do banco.

**Atributos:**

* endereço
* lista de contas

**Métodos:**

* realizar_transacao()
* adicionar_conta()

---

### PessoaFisica (Herda de Cliente)

Representa um cliente do tipo pessoa física.

**Atributos adicionais:**

* nome
* data de nascimento
* CPF

---

### Conta

Classe base para contas bancárias.

**Atributos:**

* saldo
* número da conta
* agência
* cliente
* histórico

**Métodos:**

* sacar()
* depositar()

---

### ContaCorrente (Herda de Conta)

Conta com regras específicas.

**Atributos adicionais:**

* limite de saque
* limite de quantidade de saques

---

### Historico

Armazena todas as transações realizadas.

---

### Transacao (Classe Abstrata)

Define o comportamento padrão das transações.

---

### Saque

Implementa a lógica de saque.

---

### Deposito

Implementa a lógica de depósito.

---

## Funcionalidades do Sistema

O sistema possui um menu interativo com as seguintes opções:

```
[d] Depositar
[s] Sacar
[e] Extrato
[nc] Nova conta
[lc] Listar contas
[nu] Novo usuário
[q] Sair
```

---

## Como Executar

### 1. Pré-requisitos

* Python 3 instalado

### 2. Executar o sistema

No terminal, execute:

```bash
python nome_do_arquivo.py
```

---

##  Exemplo de Uso

1. Criar um novo usuário
2. Criar uma conta vinculada ao usuário
3. Realizar depósitos
4. Realizar saques
5. Consultar extrato

---

## Conceitos Aplicados

* Classes e Objetos
* Herança (PessoaFisica → Cliente)
* Classe Abstrata (Transacao)
* Encapsulamento (uso de atributos privados)
* Polimorfismo (métodos sobrescritos)

---

## Vantagens da Abordagem

* Código mais organizado
* Fácil manutenção
* Reutilização de código
* Maior aderência a sistemas reais

---

## Possíveis Melhorias Futuras

* Interface gráfica (GUI)
* Persistência em banco de dados
* Validação de CPF
* Múltiplas contas por cliente com seleção
* API REST

---

## Autor
Desenvolvido por Anderson Nascimento (estudante de Análise e Desenvolvimento de Sistemas).

---

##  Licença

Este projeto é apenas para fins acadêmicos e profissionais. 
Ressaltando que tudo o que foi construído, não seria possível 
se não tivesse participado do Bootcamp da Luizalabs com a DIO.
