# Relatório de Execução de Teste - CT-002

## Identificação do Teste
- ID: CT-002
- Nome: Login com senha inválida
- Módulo: Autenticação (Login)
- Tipo de teste: Funcional / Negativo

---

## Objetivo
Validar que o sistema bloqueia o acesso quando uma senha inválida é informada.

---

## Ambiente de Teste
- Aplicação: SauceDemo
- URL: https://www.saucedemo.com/
- Navegador: Google Chrome
- Modo de execução: Aba anônima (Incognito)
- Sistema operacional: Windows 11
- Dados utilizados:
  - Usuário: standard_user
  - Senha: senha_errada
---

## Passos executados
1. Acessar a página de login
2. Inserir usuário válido (standard_user)
3. Inserir senha inválida (senha_errada)
4. Clicar no botão "Login"

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
evidences/ct-002-negat-senha-invalida.png

---

## Observações
A aplicação apresentou comportamento esperado ao impedir acesso com senha inválida.

---

## Responsável
Wesllem S. Campos
