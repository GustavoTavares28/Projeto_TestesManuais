# Teste Funcional de Busca (Mercado Livre)

## Informações do Teste

**Aplicação:** Mercado Livre  
**Tipo de Teste:** Teste Funcional de Busca  
**Objetivo:** Validar a funcionalidade de busca de produtos, relevância dos resultados, aplicação de filtros e ordenação.

---

## Pré-condições

- Acessar o site do Mercado Livre.
- Utilizar a barra de busca da aplicação.

---

# Cenários Executados

## 1. Buscar produto existente

### Objetivo

Validar se o sistema permite realizar uma busca e retornar produtos relacionados.

| Passo | Ação | Resultado Esperado | Resultado Obtido | Status |
|---|---|---|---|:---:|
| 1.1 | Clicar na barra de busca. | O sistema deve permitir a digitação de produtos. | A barra de busca permitiu inserir informações corretamente. | ✅ Passou |
| 1.2 | Digitar "notebook" e pressionar Enter. | O sistema deve retornar diferentes modelos de notebooks. | Foram exibidos diversos notebooks relacionados à pesquisa. | ✅ Passou |

---

## 2. Validar relevância dos resultados

### Objetivo

Verificar se os produtos retornados possuem relação adequada com o termo pesquisado.

| Passo | Ação | Resultado Esperado | Resultado Obtido | Status |
|---|---|---|---|:---:|
| 2.1 | Acessar a barra de busca. | O sistema deve permitir a digitação de produtos. | A barra de busca funcionou corretamente. | ✅ Passou |
| 2.2 | Digitar "computador" e pressionar Enter. | O sistema deve retornar computadores relacionados ao termo pesquisado. | Foram exibidos diversos periféricos de computador, não correspondendo totalmente ao produto pesquisado. | ❌ Falhou |

---

## 3. Buscar produto inexistente

### Objetivo

Validar o comportamento da aplicação ao pesquisar um termo sem resultados esperados.

| Passo | Ação | Resultado Esperado | Resultado Obtido | Status |
|---|---|---|---|:---:|
| 3.1 | Acessar a barra de busca. | O sistema deve permitir a digitação de produtos. | A barra de busca funcionou corretamente. | ✅ Passou |
| 3.2 | Digitar "abcd1234" e pressionar Enter. | O sistema deve informar que nenhum produto foi encontrado. | A aplicação apresentou produtos aleatórios ao invés de informar ausência de resultados. | ❌ Falhou |

---

## 4. Validar aplicação de filtros

### Objetivo

Verificar se os filtros disponíveis retornam resultados conforme os critérios selecionados.

| Passo | Ação | Resultado Esperado | Resultado Obtido | Status |
|---|---|---|---|:---:|
| 4.1 | Acessar a barra de busca. | O sistema deve permitir pesquisa de produtos. | A funcionalidade estava disponível. | ✅ Passou |
| 4.2 | Pesquisar "notebook". | O sistema deve retornar notebooks disponíveis. | Foram exibidos diversos notebooks. | ✅ Passou |
| 4.3 | Aplicar filtro de marca "Lenovo". | O sistema deve retornar apenas notebooks Lenovo. | Os resultados foram filtrados corretamente. | ✅ Passou |
| 4.4 | Aplicar filtro de preço até R$ 4.000,00. | O sistema deve retornar produtos dentro do limite informado. | Os resultados respeitaram o filtro aplicado. | ✅ Passou |

---

## 5. Validar ordenação por menor preço

### Objetivo

Verificar se a ordenação de produtos funciona corretamente.

| Passo | Ação | Resultado Esperado | Resultado Obtido | Status |
|---|---|---|---|:---:|
| 5.1 | Acessar a barra de busca. | O sistema deve permitir pesquisa. | A funcionalidade estava disponível. | ✅ Passou |
| 5.2 | Pesquisar "notebook". | O sistema deve retornar notebooks disponíveis. | Foram exibidos diversos notebooks. | ✅ Passou |
| 5.3 | Selecionar ordenação "menor preço". | Os notebooks deveriam ser organizados do menor valor para o maior. | O sistema exibiu produtos relacionados a notebooks com menor preço, porém não necessariamente os notebooks mais baratos. | ❌ Falhou |

---

# Resultado Geral

| Total de Validações | Passou | Falhou |
|---|---|---|
| 12 | 9 | 3 |
**Status Final:** ⚠️ Aprovado com inconsistências

---

# Bugs Identificados

Durante a execução dos testes foram encontrados defeitos relacionados à busca e ordenação de produtos.

- [BUG001 — Resultados de busca pouco relevantes](../../bug-report/BUG001-resultados-busca-relevantes.md)
- [BUG002 — Pesquisa sem resultado apresenta produtos aleatórios](../../bug-report/BUG002-produto-inexistente.md)
- [BUG003 — Ordenação por menor preço inconsistente](../../bug-report/BUG003-ordenacao-menor-preco.md)
