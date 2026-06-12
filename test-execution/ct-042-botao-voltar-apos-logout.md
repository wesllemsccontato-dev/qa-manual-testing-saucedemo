# Relatório de Execução de Teste - CT-042

## Identificação do Teste
- ID: CT-042
- Nome: Botão voltar após logout
- Módulo: Autenticação (Login)
- Tipo de teste: Funcional / Negativo

---

## Objetivo
- Validar se o sistema impede acesso direto as páginas protegidas depois de fazer logout, atraves do botão voltar do navegador.
---

## Ambiente de Teste
- Aplicação: SauceDemo
- URL: https://www.saucedemo.com/
- Navegador: Google Chrome
- Modo de execução: Aba anônima (Incognito)
- Sistema operacional: Windows 11
- Dados utilizados:
  - Usuário: standard_user
  - Senha: secret_sauce


---

## Passos executados
1. Acessar a página de login.
2. Inserir usuário valido:
   "standard_user".
3. Inserir senha valida:
   "secret_sauce".
4. Clicar no botão "Login".
5. Clicar no perfil do usuario
6. Clicar em Logout.
7. Clicar em voltar a página
---

## Resultado obtido

- O sistema bloqueou corretamente o acesso à página protegida após o logout. Ao utilizar o botão "Voltar" do navegador, o usuário permaneceu na tela de login devido à ausência de uma sessão autenticada.

"Epic sadface: You can only access '/inventory.html' when you are logged in"

O sistema destacou o erro visualmente utilizando borda vermelha e ícones de validação.

---

## Resultado esperado
- O sistema deve impedir o acesso a páginas protegidas após o encerramento da sessão, mesmo quando o usuário utiliza o botão "Voltar" do navegador.
---

## Status do teste
✔ PASSOU

---

## Evidência
- Print disponível em:
  evidences/ct-042-botao-voltar-apos-logout.png

---
## Observações
- O teste demonstra que o sistema invalida corretamente a sessão após o logout e não depende apenas do histórico de navegação do navegador para controle de acesso.
---

## Responsável
Wesllem S. Campos
