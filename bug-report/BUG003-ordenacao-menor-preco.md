# BUG003 — Ordenação por menor preço exibe produtos não correspondentes ao termo pesquisado

## Informações do Bug

**Aplicação:** Mercado Livre  
**Tipo:** Funcional  
**Severidade:** Média  
**Prioridade:** Alta  
**Status:** Aberto  
**Ambiente:** Google Chrome / Windows 10

---

## Descrição

Ao aplicar a ordenação por "Menor preço" em uma busca por notebooks, o sistema não mantém a relevância dos resultados e apresenta produtos relacionados à categoria, ao invés de ordenar apenas notebooks.

---

## Passos para Reprodução

1. Acessar a página do Mercado Livre;
2. Clicar na barra de busca;
3. Pesquisar por **"notebook"**;
4. Pressionar Enter;
5. Selecionar a ordenação **"Menor preço"**;
6. Analisar os produtos retornados.

---

## Resultado Esperado

O sistema deve ordenar os produtos correspondentes ao termo pesquisado (**notebook**) do menor para o maior preço, mantendo a relevância da busca.

---

## Resultado Encontrado

Após selecionar a ordenação por menor preço, o sistema apresenta acessórios e outros produtos relacionados à categoria de notebooks, ao invés de ordenar somente notebooks.

---

## Evidência

[Imagem — BUG003](https://www.awesomescreenshot.com/image/62003131?key=39d83d2fc7bc269c36229745c3709e8b)