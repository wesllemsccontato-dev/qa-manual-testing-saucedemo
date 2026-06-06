# Projeto de Testes Manuais - SauceDemo

## Objetivo

Este projeto foi desenvolvido com o objetivo de demonstrar conhecimentos práticos em Quality Assurance (QA), incluindo planejamento, execução e documentação de testes manuais em uma aplicação web.

Durante o projeto foram aplicadas técnicas de validação funcional, testes negativos, segurança básica, usabilidade, acessibilidade, compatibilidade e gerenciamento de evidências.

---

## Aplicação Testada

* Sistema: SauceDemo
* URL: https://www.saucedemo.com/

---

## Escopo dos Testes

### Funcionais

* Login válido
* Login inválido
* Logout
* Navegação entre páginas
* Validação de mensagens de erro

### Segurança

* SQL Injection
* Cross-Site Scripting (XSS)
* Acesso sem autenticação
* Acesso por URL direta
* Controle de sessão após logout

### Usabilidade e Acessibilidade

* Navegação por TAB
* Login utilizando ENTER
* Avaliação de foco visual
* Análise de mensagens de erro
* Avaliação de experiência do usuário (UX)

### Sessão

* Persistência da sessão após atualização da página
* Validação de logout
* Proteção de páginas autenticadas

### Performance Básica

* Carregamento da tela de login

### Compatibilidade

* Google Chrome
* Microsoft Edge

---

## Artefatos Produzidos

* Plano de Testes
* Casos de Teste
* Relatórios de Execução
* Bug Reports
* Evidências de Teste
* Matriz de Compatibilidade

---

## Estrutura do Projeto

```text
├── README.md
├── test-cases
├── test-executions
├── bug-reports
└── evidences
```

---

## Compatibilidade Validada

| ID     | Navegador      | Resultado  |
| ------ | -------------- | ---------- |
| CT-095 | Google Chrome  | ✔ Aprovado |
| CT-097 | Microsoft Edge | ✔ Aprovado |

---

## Ferramentas Utilizadas

* GitHub
* Markdown
* Google Chrome
* Microsoft Edge
* Windows 11

---

## Resultados

* Casos de teste executados com sucesso
* Evidências documentadas
* Bugs reportados e classificados
* Cobertura de testes funcionais, segurança, acessibilidade, sessão e compatibilidade

---

## Autor

Wesllem S. Campos

Projeto desenvolvido como parte da preparação para atuação profissional na área de Quality Assurance (QA).
