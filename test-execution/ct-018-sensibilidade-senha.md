# Relatório de Execução de Teste - CT-018

## Identificação do Teste
- ID: CT-018
- Nome: Sensibilidade da senha
- Módulo: Autenticação (Login)
- Tipo de teste: Funcional / Negativo

---

## Objetivo
- Validar se o sistema diferencia letras maiúsculas e minúsculas no campo senha durante autenticação.
---

## Ambiente de Teste
- Aplicação: SauceDemo
- URL: https://www.saucedemo.com/
- Navegador: Google Chrome
- Modo de execução: Aba anônima (Incognito)
- Sistema operacional: Windows 11
- Dados utilizados:
  - Usuário: standard_user
  - Senha: SECRET_SAUCE

---

## Passos executados
1. Acessar a página de login.
2. Inserir usuário valido:
   "standard_user".
3. Ativar a tecla Caps Lock
4. Inserir senha com capitalização alterada:
"SECRET_SAUCE".
5. Clicar no botão "Login".

---

## Resultado obtido

- Sistema bloqueou autenticação corretamente ao identificar diferença de capitalização no campo senha e apresentou mensagem de erro padrão de autenticação.

"Epic sadface: Username and password do not match any user in this service"

O sistema destacou o erro visualmente utilizando borda vermelha e ícones de erro.

---

## Resultado esperado
- Sistema deve tratar o campo senha como case sensitive, bloqueando autenticação quando a capitalização estiver incorreta.
- Bloquear o acesso, informando o erro com mensagen.
---

## Status do teste
✔ PASSOU

---

## Evidência
- Print disponível em:
  evidences/ct-018-negat-sensibilidade-senha.png

---
## Observações
- O sistema apresentou comportamento esperado ao tratar a senha como case sensitive. Entretanto, a ausência de aviso visual para Caps Lock ativado pode contribuir para erros involuntários de autenticação, cenário relacionado ao BUG-005.


## Responsável
Wesllem S. Campos
