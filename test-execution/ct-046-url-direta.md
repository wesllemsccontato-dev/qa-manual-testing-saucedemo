# Relatório de Execução de Teste - CT-046

## Identificação do Teste
- ID: CT-046
- Nome: URL direta
- Módulo: Autenticação (Login)
- Tipo de teste: Funcional / Negativo

---

## Objetivo
- Validar que páginas protegidas não podem ser acessadas diretamente através da URL após o encerramento da sessão.
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
2. Fazer Login com:
   Usuario : "standard_user".
   Senha:  "secret_sauce".
3. Confirmar acesso à página de produto
4. Copiar a URL protegida.
5. Fazer Logout.
6. Colar novamente na barra do navegador.
7. Pressionar ENTER.


## Resultado obtido
- O sistema bloqueou corretamente o acesso à página protegida após o logout. Ao tentar acessar pela URL direta, o usuário permaneceu na tela de login devido à ausência de uma sessão autenticada.

"Epic sadface: You can only access '/inventory.html' when you are logged in"

- O sistema destacou o erro visualmente utilizando borda vermelha e ícones de validação.


---

## Resultado esperado
- A sessão deve permanecer encerrada após o logout.
- O sistema deve impedir o acesso a páginas protegidas sem autenticação.
- O sistema deve redirecionar o usuário para a tela de login e informar a ausência de uma sessão válida

---

## Status do teste
✔ PASSOU

---


## Evidência
- Print disponível em:
  evidences/ct-46-url-direta.png
  
---

## Observações
- O teste demonstra que o sistema invalida corretamente a sessão após o logout e não depende apenas do histórico de navegação do navegador para controle de acesso.


## Responsável
Wesllem S. Campos
