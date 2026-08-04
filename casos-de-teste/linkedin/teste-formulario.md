# Teste de Formulário de Cadastro (LinkedIn)

## Informações do Teste

**Aplicação:** LinkedIn  
**Tipo de Teste:** Teste Funcional de Formulário  
**Objetivo:** Validar os comportamentos do formulário de cadastro, verificando preenchimentos válidos, inválidos, mensagens de erro e comportamento dos componentes.

---

## Pré-condições

- Acessar o site do LinkedIn.
- Acessar a opção **"Criar conta"**.

---

# Cenários Executados

## 1. Abrir formulário de cadastro

### Objetivo
Validar se o formulário de criação de conta é exibido corretamente.

| Passo | Ação | Resultado Esperado | Resultado Obtido | Status |
|---|---|---|---|:---:|
| 1.1 | Clicar em **"Criar conta"** | O formulário de cadastro deve ser exibido corretamente. | O formulário de cadastro foi exibido corretamente. | ✅ Passou |

---

## 2. Validar campo de e-mail com formato inválido

### Objetivo
Verificar se o sistema realiza validação de formato do e-mail informado.

| Passo | Ação | Resultado Esperado | Resultado Obtido | Status |
|---|---|---|---|:---:|
| 2.1 | Acessar a tela de cadastro. | O formulário deve ser exibido corretamente. | O formulário foi exibido corretamente. | ✅ Passou |
| 2.2 | Informar um e-mail inválido e clicar em **"Continuar"**. | O sistema deve impedir o avanço e informar que o e-mail é inválido. | Foi exibida a mensagem: "Insira um e-mail ou número de celular válido." O sistema bloqueou o avanço. | ✅ Passou |

---

## 3. Validar campos obrigatórios vazios

### Objetivo
Verificar o comportamento da aplicação quando campos obrigatórios não são preenchidos.

| Passo | Ação | Resultado Esperado | Resultado Obtido | Status |
|---|---|---|---|:---:|
| 3.1 | Acessar a tela de cadastro. | O formulário deve ser exibido corretamente. | O formulário foi exibido corretamente. | ✅ Passou |
| 3.2 | Deixar campos obrigatórios vazios e clicar em **"Continuar"**. | O sistema deve impedir o avanço e apresentar mensagens de validação. | O sistema bloqueou o avanço e exibiu mensagens de validação. | ✅ Passou |

---

## 4. Validar e-mail com letras maiúsculas

### Objetivo
Verificar o tratamento do sistema para e-mails contendo letras maiúsculas.

| Passo | Ação | Resultado Esperado | Resultado Obtido | Status |
|---|---|---|---|:---:|
| 4.1 | Acessar a tela de cadastro. | O formulário deve ser exibido corretamente. | O formulário foi exibido corretamente. | ✅ Passou |
| 4.2 | Informar e-mail com letras maiúsculas e clicar em **"Continuar"**. | O sistema deve aceitar o e-mail caso seja válido. | O sistema aceitou o e-mail e realizou o tratamento das letras maiúsculas. | ✅ Passou |

---

## 5. Validar regras de senha

### Objetivo
Verificar o comportamento do formulário ao receber diferentes combinações de senha.

| Passo | Ação | Resultado Esperado | Resultado Obtido | Status |
|---|---|---|---|:---:|
| 5.1 | Acessar a tela de cadastro. | O formulário deve ser exibido corretamente. | O formulário foi exibido corretamente. | ✅ Passou |
| 5.2 | Informar senha curta, sem números ou sem letras. | O sistema deve validar as regras de senha e apresentar mensagens quando necessário. | O sistema rejeitou senhas abaixo do tamanho mínimo. Senhas sem números ou letras foram aceitas conforme regras aplicadas. | ✅ Passou |

---

## 6. Validar comportamento do botão "Continuar"

### Objetivo
Verificar disponibilidade e funcionamento do botão durante o preenchimento do formulário.

| Passo | Ação | Resultado Esperado | Resultado Obtido | Status |
|---|---|---|---|:---:|
| 6.1 | Acessar a tela de cadastro. | O formulário deve ser exibido corretamente. | O formulário foi exibido corretamente. | ✅ Passou |
| 6.2 | Observar o botão antes do preenchimento dos campos. | O botão deve estar visível e disponível para interação. | O botão permaneceu disponível corretamente. | ✅ Passou |
| 6.3 | Clicar em "Continuar" com campos vazios. | O sistema deve impedir o avanço e exibir mensagens de validação. | O sistema bloqueou o avanço e exibiu mensagens de validação. | ✅ Passou |
| 6.4 | Preencher os campos corretamente e clicar em "Continuar". | O botão deve permitir avançar para a próxima etapa do cadastro. | O sistema permitiu o prosseguimento para a próxima etapa. | ✅ Passou |

---

## Resultado Geral

| Total de Testes | Passou | Falhou |
|---|---|---|
| 10 | 10 | 0 |

**Status Final:** ✅ Aprovado

---

## Observações

Durante a execução dos testes foi identificado um comportamento que não pôde ser confirmado como defeito.

- ⚠️ **ERRO001 — Cadastro prossegue sem confirmação imediata de e-mail**, conforme as regras atuais da aplicação. Recomenda-se avaliar se o comportamento está de acordo com os requisitos de segurança.
  ➡️ [Visualizar registro](../lista-erros-encontrados/erros-em-analise/ERRO001-confirmacao-email.md)