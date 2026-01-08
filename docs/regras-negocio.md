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

5.1 Apenas cooperados com cadastro completo e status ATIVO podem realizar simulação de empréstimo.

5.2 A simulação de empréstimo não implica na contratação do crédito.

5.3 O cooperado deve informar obrigatoriamente:
- Valor do empréstimo
- Quantidade de parcelas

5.4 O valor mínimo do empréstimo deve ser maior que zero.

5.5 O sistema deve validar se o valor solicitado está dentro do limite de crédito do cooperado.

5.6 O número de parcelas deve respeitar os limites definidos pela política de crédito da cooperativa.

5.7 A simulação deve apresentar ao cooperado:
- Valor total do empréstimo
- Valor da parcela
- Taxa de juros aplicada

5.8 O sistema deve permitir múltiplas simulações sem obrigatoriedade de contratação.

5.9 Caso alguma regra de simulação não seja atendida, o sistema deve exibir mensagem clara informando o motivo da reprovação.

## 6. Regras de Contratação

6.1 A contratação do empréstimo só pode ocorrer após uma simulação válida realizada pelo cooperado.

6.2 Apenas cooperados com cadastro completo e status ATIVO podem contratar empréstimos.

6.3 O cooperado deve confirmar explicitamente a contratação do empréstimo.

6.4 O sistema deve validar novamente as regras de crédito no momento da contratação.

6.5 Não deve ser permitida a contratação duplicada de um mesmo empréstimo.

6.6 Após a confirmação da contratação, o sistema deve:
- Gerar o contrato do empréstimo
- Registrar a operação no sistema
- Agendar as parcelas para pagamento

6.7 O contrato deve conter, no mínimo:
- Dados do cooperado
- Valor contratado
- Taxa de juros
- Quantidade e valor das parcelas
- Data de vencimento da primeira parcela

6.8 Caso ocorra falha durante a contratação, o sistema deve cancelar a operação e informar o cooperado.


## 7. Regras de Exceção e Erros
