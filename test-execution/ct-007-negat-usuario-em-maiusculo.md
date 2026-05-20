# Relatório de Execução de Teste - CT-007

## Identificação do Teste
- ID: CT-007
- Nome: Letras maiúsculas no  Usuário 
- Módulo: Autenticação (Login)
- Tipo de teste: Funcional / Negativo

---

## Objetivo
Validar que o sistema bloqueia o acesso quando ha letras maiúsculas inceridos no usuário.

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
   "STANDARD_USER".
3. Inserir senha válida:
"secret_sauce".
4. Clicar no botão "Login".

---

## Resultado obtido
- Login não realizado
- Usuário permaneceu na tela de login
- Sistema apresentou mensagem de erro 

---

## Resultado esperado
- Sistema deve bloquear login inválido
- Mensagem de erro deve ser exibida ao usuário

---

## Status do teste
✔ PASSOU

---

## Evidência
Print disponível em:
evidences/ct-007-negat-usuario-em-maiusculo.png

---

## Observações
A aplicação apresentou comportamento esperado ao impedir acesso quando letras maiúsculas são inceridos no usuário.

---

## Responsável
Wesllem S. Campos
