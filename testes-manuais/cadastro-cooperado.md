
# Testes Manuais – Cadastro de Cooperado

## CT-01 – Cadastro com dados válidos
**Objetivo:** Validar o cadastro de cooperado com dados obrigatórios preenchidos.

**Pré-condições:**
- Cooperado maior de 18 anos
- CPF válido e não cadastrado

**Passos:**
1. Informar nome completo
2. Informar CPF válido
3. Informar data de nascimento
4. Informar renda mensal
5. Informar agência de vínculo
6. Confirmar cadastro

**Resultado Esperado:**
- Cadastro realizado com sucesso

---

## CT-02 – Cadastro com CPF inválido
**Objetivo:** Validar mensagem de erro ao informar CPF inválido.

**Pré-condições:**
- Nenhuma

**Passos:**
1. Informar CPF inválido
2. Preencher demais dados obrigatórios
3. Confirmar cadastro

**Resultado Esperado:**
- Sistema exibe mensagem de erro informando CPF inválido

---

## CT-03 – Cadastro com CPF duplicado
**Objetivo:** Impedir cadastro de cooperado com CPF já existente.

**Pré-condições:**
- CPF já cadastrado no sistema

**Passos:**
1. Informar CPF já existente
2. Preencher demais dados obrigatórios
3. Confirmar cadastro

**Resultado Esperado:**
- Sistema bloqueia cadastro e informa duplicidade de CPF
