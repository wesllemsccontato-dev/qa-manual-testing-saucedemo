# Relatório de Execução de Teste - CT-003

## Identificação do Teste
- ID: CT-003
- Nome: Usuário inválido
- Módulo: Autenticação (Login)
- Tipo de teste: Funcional / Negativo

---

## Objetivo
Validar que o sistema bloqueia o acesso quando uma usuário inválido é informada.

---

## Ambiente de Teste
- Aplicação: SauceDemo
- URL: https://www.saucedemo.com/
- Navegador: Google Chrome
- Modo de execução: Aba anônima (Incognito)
- Sistema operacional: Windows 11
- Dados utilizados:
  - Usuário: usuario_fake
  - Senha: secret_sauce
---

## Passos executados
1. Acessar a página de login
2. Inserir usuário válido (usuario_fake)
3. Inserir senha válida (secret_sauce)
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
evidences/ct-003-negat-usuario-invalido.png

---

## Observações
A aplicação apresentou comportamento esperado ao impedir acesso com senha inválida.

---

## Responsável
Wesllem S. Campos
