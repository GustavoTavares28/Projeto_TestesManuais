# BUG002 — Busca por produto inexistente retorna produtos não relacionados

## Informações do Bug

**Aplicação:** Mercado Livre  
**Tipo:** Funcional  
**Severidade:** Média  
**Prioridade:** Média  
**Status:** Aberto  
**Ambiente:** Google Chrome / Windows 10

---

## Descrição

Ao realizar uma busca utilizando um termo inexistente, o sistema não informa que nenhum resultado foi encontrado e apresenta produtos sem relação com o termo pesquisado.

---

## Passos para Reprodução

1. Acessar a página do Mercado Livre;
2. Clicar na barra de busca;
3. Digitar **"abcd1234"**;
4. Pressionar Enter;
5. Analisar os resultados apresentados.

---

## Resultado Esperado

O sistema deve informar que nenhum resultado foi encontrado para o termo pesquisado ou apresentar uma mensagem equivalente.

---

## Resultado Encontrado

O site apresenta produtos aleatórios, sem relação com o termo pesquisado.

---

## Evidência

[Imagem — BUG002](https://www.awesomescreenshot.com/image/62003304?key=8d8b98e831a171db2f36835810d19db1)