# Alterações aplicadas — Skill `arquitetura-cypress`

Data: 2026-06-18

Resumo das mudanças realizadas no arquivo `.github/skills/arquitetura/SKILL.md`:

- Escopo E2E: adicionada frase explicitando que a skill se aplica somente a testes E2E em `cypress/e2e/` e que não deve gerar testes de componente a menos que solicitado.
- Segurança de seletores: incluída regra para **não inventar** seletores/rotas/fixtures; pedir ao usuário os seletores/rotas/textos exatos se não existirem.
- Tratamento de erro: adicionada instrução para parar e pedir esclarecimentos quando os seletores/fixtures/rotas necessários não forem fornecidos.
- Estrutura do projeto: simplificada a estrutura de exemplo para `cypress/e2e/`, `cypress/fixtures/`, `cypress/support/e2e.ts` e `cypress.config.ts`; removido `plugins/index.ts` do exemplo.
- Configuração: removido o bloco de `component` config do exemplo `cypress.config.ts` para evitar misturar convenções de component testing.
- Conflito de comandos de login: renomeado o comando UI para `loginUI` e mantida a versão `login` que usa `cy.session()`; atualizadas as declarações `Chainable` para refletir `loginUI`, `loginByApi` e `login`.
- Boas práticas: substituída a lista extensa por 4 regras mandatórias e adicionada orientação para priorizar a regra mais específica quando houver conflito.
- Component Testing: inserida nota indicando que pedidos de component tests devem ser redirecionados ao skill/component-testing apropriado.

Arquivos modificados:

- `.github/skills/arquitetura/SKILL.md` — edits aplicadas inline.

Próximo passo opcional:

- Comitar as mudanças no branch `main` e/ou abrir um PR. Deseja que eu crie o commit?