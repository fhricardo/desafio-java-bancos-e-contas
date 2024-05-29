
# Desafio: Sistema de Gerenciamento de Contas Bancárias

## Objetivo:
Desenvolver um sistema simples para gerenciar diferentes tipos de contas bancárias usando herança, polimorfismo e coleções em Java.

### Instruções:

1. **Classe Base `ContaBancaria`**:
    - Atributos: `numeroConta`, `titular`, `saldo`.
    - Métodos: Construtor, getters e setters, `depositar` (adicionar ao saldo), `sacar` (subtrair do saldo, se houver saldo suficiente), `exibirInfo` (exibir informações da conta).

2. **Classes Derivadas `ContaCorrente` e `ContaPoupanca`**:
    - `ContaCorrente`: Adicionar atributo `taxaManutencao`.
    - `ContaPoupanca`: Adicionar atributo `taxaJuros`.

3. **Sobrescrever o método `exibirInfo` nas classes derivadas** para exibir as informações adicionais.

4. **Classe `Banco`**:
    - Atributo: Lista de contas (`ArrayList<ContaBancaria>`).
    - Métodos: `adicionarConta`, `exibirTodasContas`, `buscarContaPorNumero`, `removerContaPorNumero`.

5. **Classe Principal `Main`**:
    - Criar instâncias de `ContaCorrente` e `ContaPoupanca`.
    - Adicionar as contas ao banco.
    - Exibir as informações de todas as contas no banco.
    - Realizar operações de depósito e saque, e exibir o saldo atualizado.

#### Requisitos Extras:
- Implementar um método para calcular e aplicar a taxa de juros nas contas poupança.
- Implementar um método para cobrar a taxa de manutenção nas contas correntes
