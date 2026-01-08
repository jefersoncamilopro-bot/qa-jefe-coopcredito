por que me apresentou essas regras anteriormente ?
está faltando regras?

# Regras de Negócio – Sistema de Empréstimos para Cooperados

## 1. Objetivo do Sistema
Sistema destinado à simulação e contratação de empréstimos por cooperados da cooperativa de crédito.

## 2. Tipos de Usuário
- Cooperado
- Operador Interno (Agência / Backoffice)
- Sistema (Integrações)

## 3. Fluxo Principal do Sistema
1. Cooperado realiza cadastro ou atualização cadastral
2. Cooperado simula empréstimo
3. Sistema valida regras de crédito
4. Cooperado confirma contratação
5. Sistema gera contrato e agenda pagamento

## 4. Regras de Cadastro de Cooperado

4.1 O cooperado deve possuir CPF válido e único no sistema.

4.2 O cooperado deve ter idade mínima de 18 anos.

4.3 O cooperado deve estar com status ATIVO na cooperativa para realizar cadastro, simulação ou contratação de empréstimos.

4.4 O cadastro do cooperado deve conter obrigatoriamente:
- Nome completo
- CPF
- Data de nascimento
- Renda mensal
- Agência de vínculo

4.5 Cooperados com cadastro incompleto não podem simular empréstimos.

4.6 Não é permitido o cadastro de cooperados com CPF já existente no sistema.

4.7 O sistema deve permitir atualização cadastral apenas para cooperados ativos.

## 5. Regras de Simulação de Empréstimo

## 6. Regras de Contratação

## 7. Regras de Exceção e Erros
