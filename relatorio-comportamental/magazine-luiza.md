# 📑 Relatório Comportamental — Magazine Luiza

## Objetivo

Avaliar o comportamento do formulário de login da aplicação, comparando os resultados esperados com os comportamentos observados durante a execução dos testes.

---

## Resumo

| Cenário | Comportamento Esperado | Comportamento Observado | Status |
| --- | --- | --- | :---: |
| Login com senha incorreta | Impedir o login e informar credenciais inválidas. | O sistema impediu o login e exibiu mensagem de erro. | ✅ Conforme esperado |
| E-mail sem "@" | Validar o formato do e-mail. | O sistema identificou o formato inválido. | ✅ Conforme esperado |
| Senha vazia | Solicitar o preenchimento da senha. | O sistema solicitou o preenchimento. | ✅ Conforme esperado |
| E-mail vazio | Solicitar o preenchimento do e-mail. | O sistema solicitou o preenchimento. | ✅ Conforme esperado |
| Mostrar senha | Exibir e ocultar a senha corretamente. | Funcionou conforme esperado. | ✅ Conforme esperado |
| Senha abaixo do mínimo | Informar que a senha não atende ao tamanho mínimo. | O sistema exibiu apenas a mensagem **"Dados inválidos"**. | ⚠️ Em análise |

---

## Conclusão

Durante a execução dos testes, a funcionalidade de login apresentou comportamento consistente na maioria dos cenários avaliados, atendendo às expectativas para validação de credenciais, formato de e-mail, obrigatoriedade de campos e exibição da senha.

Foi observada uma divergência no cenário de validação de senha abaixo do tamanho mínimo. Nesse caso, o sistema apresentou apenas uma mensagem genérica (**"Dados inválidos"**), sem informar especificamente que o requisito de tamanho mínimo não havia sido atendido.

Como não foi possível consultar os requisitos funcionais ou critérios de aceitação da aplicação, **não há evidências suficientes para classificar esse comportamento como um defeito**. Recomenda-se validar a regra de negócio com a documentação do sistema ou com a equipe responsável para confirmar se o comportamento está de acordo com o esperado.

➡️ Para mais detalhes, consulte a **Lista de Erros Encontrados**:
[ERRO002 — Mensagem genérica para validação de senha](../lista-erros-encontrados/erros-em-analise/ERRO002-validacao-senha.md)