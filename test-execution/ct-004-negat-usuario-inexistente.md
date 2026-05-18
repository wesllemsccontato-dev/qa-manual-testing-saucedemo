# Relatório de Execução de Teste - CT-004

## Identificação do Teste
- ID: CT-004
- Nome: Usuário Inexistente
- Módulo: Autenticação (Login)
- Tipo de teste: Funcional / Negativo

---

## Objetivo
Validar que o sistema bloqueia o acesso quando uma usuário inexistente é informado.

---

## Ambiente de Teste
- Aplicação: SauceDemo
- URL: https://www.saucedemo.com/
- Navegador: Google Chrome
- Modo de execução: Aba anônima (Incognito)
- Sistema operacional: Windows 11
- Dados utilizados:
  - Usuário: usuario_inexistente
  - Senha: secret_sauce
---

## Passos executados
1. Acessar a página de login
2. Inserir usuário inexistente (usuario_inexistente)
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
evidences/ct-004-negat-usuario-inexistente.png

---

## Observações
A aplicação apresentou comportamento esperado ao impedir acesso com senha inválida.

---

## Responsável
Wesllem S. Campos
