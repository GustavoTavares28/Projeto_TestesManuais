# ERRO002 — Cadastro prossegue sem confirmação imediata de e-mail

## Informações

**Sistema testado:** LinkedIn (linkedin.com)  
**Data da execução:** 20/07/2026  
**Categoria:** Fluxo de Cadastro  
**Severidade:** Em análise  
**Status:** Observação

---

## Descrição

Durante os testes do fluxo de cadastro, foi observado que o processo pôde prosseguir sem a confirmação imediata do e-mail por meio do código de verificação.

---

## Resultado Esperado

O sistema deve solicitar a confirmação do e-mail conforme definido no fluxo de cadastro da aplicação.

---

## Resultado Encontrado

O cadastro permitiu avançar sem a validação imediata do e-mail através do código de confirmação.

---

## Análise

Não foi possível confirmar se esse comportamento faz parte do fluxo previsto da aplicação ou se representa uma falha.

Recomenda-se validação adicional.

---

## Evidência

[ERRO001](https://www.awesomescreenshot.com/video/54764742?key=7bad2018b89c18c5f6922493f4c09fda)