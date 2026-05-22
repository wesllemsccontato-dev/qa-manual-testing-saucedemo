# Relatório de Execução de Teste - CT-012

## Identificação do Teste
- ID: CT-007
- Nome: Copiar e colar senha
- Módulo: Autenticação (Login)
- Tipo de teste: Funcional / Positivo

---

## Objetivo
Validar que o usuário consegue realizar login com a senha incerida pelo comandos coíar e colar.

---

## Ambiente de Teste
- Aplicação: SauceDemo
- URL: https://www.saucedemo.com/
- Navegador: Google Chrome
- Modo de execução: Aba anônima (Incognito)
- Sistema operacional: Windows 11
- Dados utilizados:
  - Usuário: STANDARD_USER
  - Senha: secret_sauce
---

## Passos executados
1. Acessar a página de login.
2. Inserir espaços depois do usuário:
   "standard_user".
3. Copiar a colar a senha:
"secret_sauce".
4. Clicar no botão "Login".

---

## Resultado obtido
- Login realizado, usuário foi redirecionado com sucesso para a página de inventário
- URL exibida: https://www.saucedemo.com/inventory.html
- Lista de produtos carregada corretamente na tela

---

## Resultado esperado
- Usuário deve realizar login com sucesso
- Sistema deve redirecionar para a página de produtos

---

## Status do teste
✔ PASSOU

---

## Evidência
Print disponível em:
evidences/ct-012-posit-copiar-colar-senha.png

---

## Observações
A aplicação apresentou comportamento esperado ao permitir acesso quando a senha é inserida atraves de dos comandos copiar e colar.

---

## Responsável
Wesllem S. Campos
