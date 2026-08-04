# Teste de Interface (Amazon)

## Informações do Teste

**Aplicação:** Amazon  
**Tipo de Teste:** Teste de Interface (UI)  
**Objetivo:** Validar elementos visuais, consistência da interface, funcionamento de componentes e experiência de navegação do usuário.

---

## Pré-condições

- Acessar o site da Amazon.

---

# Cenários Executados

## 1. Validar barra de busca, menu e botão de login

### Objetivo

Verificar se os principais elementos de navegação estão visíveis e funcionando corretamente.

| Passo | Ação | Resultado Esperado | Resultado Obtido | Status |
|---|---|---|---|:---:|
| 1.1 | Verificar barra de busca | A barra de busca deve estar visível na página inicial. | A barra de busca está visível e bem posicionada para o usuário. | ✅ Passou |
| 1.2 | Realizar pesquisa utilizando a barra de busca | O sistema deve permitir pesquisar produtos. | A barra de busca funciona corretamente. | ✅ Passou |
| 1.3 | Verificar menu principal | O menu deve ser exibido corretamente com opções de navegação. | O menu principal foi exibido corretamente. | ✅ Passou |
| 1.4 | Verificar botão "Faça seu login" | O botão deve estar visível e acessível ao usuário. | O botão está visível e possui destaque visual para chamar atenção do usuário. | ✅ Passou |
| 1.5 | Clicar no botão "Faça seu login" | O usuário deve ser direcionado para a página de login. | O sistema realizou o redirecionamento corretamente. | ✅ Passou |

---

## 2. Validar alinhamentos, espaçamentos e contraste

### Objetivo

Verificar a consistência visual dos elementos da interface.

| Passo | Ação | Resultado Esperado | Resultado Obtido | Status |
|---|---|---|---|:---:|
| 2.1 | Validar alinhamento dos elementos | Os componentes devem estar alinhados, sem sobreposição ou cortes. | Os elementos apresentam bom alinhamento visual. | ✅ Passou |
| 2.2 | Validar espaçamento entre componentes | Os elementos devem possuir espaçamento uniforme. | Os espaçamentos apresentam boa organização visual. | ✅ Passou |
| 2.3 | Validar contraste entre texto e fundo | Os textos devem possuir contraste adequado para leitura. | Os textos apresentam boa legibilidade. | ✅ Passou |

---

## 3. Validar banners e carrosséis

### Objetivo

Verificar o carregamento e funcionamento dos elementos visuais rotativos.

| Passo | Ação | Resultado Esperado | Resultado Obtido | Status |
|---|---|---|---|:---:|
| 3.1 | Verificar carregamento do banner principal | O banner deve ser exibido sem falhas ou distorções. | O banner principal carregou corretamente. | ✅ Passou |
| 3.2 | Verificar imagens do carrossel | Todas as imagens devem carregar sem erros de exibição. | As imagens foram carregadas corretamente. | ✅ Passou |
| 3.3 | Validar troca de banners | O carrossel deve alternar automaticamente ou manualmente sem falhas. | O carrossel realizou a troca dos banners corretamente. | ✅ Passou |
| 3.4 | Verificar imagens quebradas | Nenhuma imagem deve apresentar falha de carregamento. | Foi identificada uma falha momentânea em uma imagem, porém voltou a funcionar posteriormente. Não foi possível confirmar se a causa estava relacionada ao sistema ou conexão. | ⚠️ Observação |

---

## 4. Validar menu dropdown "Contas e Listas"

### Objetivo

Verificar o comportamento do menu suspenso durante a interação do usuário.

| Passo | Ação | Resultado Esperado | Resultado Obtido | Status |
|---|---|---|---|:---:|
| 4.1 | Posicionar o cursor sobre "Contas e Listas" | O menu dropdown deve ser exibido automaticamente. | O menu dropdown foi exibido corretamente. | ✅ Passou |
| 4.2 | Validar conteúdo do menu dropdown | O menu deve apresentar textos legíveis, opções corretas e boa organização visual. | O menu apresentou todas as opções esperadas, sem erros visuais ou de texto. | ✅ Passou |

---

# Resultado Geral

| Total de Validações | Aprovados | Observações |
|---|---|---|
| 14 | 13 | 1 comportamento observado sem confirmação de defeito |

**Status Final:** ✅ Aprovado