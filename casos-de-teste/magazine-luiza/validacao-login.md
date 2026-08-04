# Teste de Validação de Login (Magazine Luiza)

## Informações do Teste

**Aplicação:** Magazine Luiza  
**Tipo de Teste:** Teste Funcional de Login  
**Objetivo:** Validar o comportamento do formulário de login, verificando entradas válidas, inválidas, campos obrigatórios, visibilidade de senha e regras de validação.

---

## Pré-condições

- Acessar o site da Magazine Luiza.
- Acessar a tela de login.

---

# Cenários Executados

## 1. Login com e-mail correto e senha incorreta

### Objetivo
Validar o comportamento do sistema ao informar credenciais inválidas.

| Passo | Ação | Resultado Esperado | Resultado Obtido | Status |
|---|---|---|---|:---:|
| 1.1 | Acessar a tela de login. | A tela deve ser exibida corretamente. | Tela carregada corretamente. | ✅ Passou |
| 1.2 | Informar e-mail válido, senha incorreta e clicar em "Continuar". | O sistema deve impedir o login e informar credenciais inválidas. | O login foi bloqueado e uma mensagem de credenciais inválidas foi exibida. | ✅ Passou |

---

## 2. Validar e-mail sem caractere "@"

### Objetivo
Verificar se o sistema identifica formatos inválidos de e-mail.

| Passo | Ação | Resultado Esperado | Resultado Obtido | Status |
|---|---|---|---|:---:|
| 2.1 | Acessar a tela de login. | A tela deve ser exibida corretamente. | Tela carregada corretamente. | ✅ Passou |
| 2.2 | Informar e-mail sem "@" e clicar em "Continuar". | O sistema deve impedir o login e apresentar mensagem de validação. | O sistema identificou o formato inválido e bloqueou o login. | ✅ Passou |

---

## 3. Validar senha vazia

### Objetivo
Verificar se o sistema impede o login sem preenchimento da senha.

| Passo | Ação | Resultado Esperado | Resultado Obtido | Status |
|---|---|---|---|:---:|
| 3.1 | Acessar a tela de login. | A tela deve ser exibida corretamente. | Tela carregada corretamente. | ✅ Passou |
| 3.2 | Deixar o campo senha vazio e clicar em "Continuar". | O sistema deve solicitar o preenchimento da senha. | O sistema bloqueou o login e solicitou o preenchimento. | ✅ Passou |

---

## 4. Validar e-mail vazio

### Objetivo
Verificar se o sistema impede o login sem preenchimento do e-mail.

| Passo | Ação | Resultado Esperado | Resultado Obtido | Status |
|---|---|---|---|:---:|
| 4.1 | Acessar a tela de login. | A tela deve ser exibida corretamente. | Tela carregada corretamente. | ✅ Passou |
| 4.2 | Deixar o campo e-mail vazio e clicar em "Continuar". | O sistema deve solicitar o preenchimento do e-mail. | O sistema bloqueou o login e solicitou o preenchimento. | ✅ Passou |

---

## 5. Validar funcionalidade "Mostrar senha"

### Objetivo
Verificar o comportamento da exibição e ocultação da senha.

| Passo | Ação | Resultado Esperado | Resultado Obtido | Status |
|---|---|---|---|:---:|
| 5.1 | Acessar a tela de login. | A tela deve ser exibida corretamente. | Tela carregada corretamente. | ✅ Passou |
| 5.2 | Informar uma senha no campo correspondente. | A senha deve permanecer mascarada inicialmente. | A senha permaneceu oculta. | ✅ Passou |
| 5.3 | Clicar no ícone "Mostrar senha". | A senha deve ser exibida e voltar a ser ocultada ao clicar novamente. | A senha ficou visível e retornou ao modo mascarado ao ocultar. | ✅ Passou |

---

## 6. Validar limite mínimo de caracteres da senha

### Objetivo
Verificar se o sistema realiza validação adequada do tamanho mínimo da senha.

| Passo | Ação | Resultado Esperado | Resultado Obtido | Status |
|---|---|---|---|:---:|
| 6.1 | Acessar a tela de login. | A tela deve ser exibida corretamente. | Tela carregada corretamente. | ✅ Passou |
| 6.2 | Informar senha abaixo do limite mínimo e clicar em "Continuar". | O sistema deve informar que a senha não atende ao tamanho mínimo. | O sistema exibiu apenas a mensagem genérica "Dados inválidos", sem informar o requisito de tamanho mínimo. | ❌ Falhou |
| 6.3 | Informar senha dentro do limite mínimo e clicar em "Continuar". | O sistema deve aceitar o formato da senha e continuar a validação. | O sistema não realizou validação específica do tamanho da senha, exibindo apenas mensagem genérica. | ❌ Falhou |

---

# Resultado Geral

| Total de Testes | Passou | Falhou |
|---|---|---|
| 13 | 11 | 2 |

**Status Final:** ⚠️ Aprovado com inconsistências

---

## Observação

Os passos 6.2 e 6.3 foram classificados como **Falhou** por apresentarem comportamento diferente do resultado esperado definido para o teste.

Entretanto, **não foi possível confirmar se esse comportamento representa um defeito da aplicação**, pois não houve acesso aos requisitos funcionais ou critérios de aceitação referentes à política de validação de senha.

O caso foi registrado para acompanhamento em:

➡️ [ERRO002 — Mensagem genérica para validação de senha](../../lista-erros-encontrados/erros-em-analise/ERRO002-validacao-senha.md)