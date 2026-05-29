# Relatório de Execução de Teste - CT-040

## Identificação do Teste
- ID: CT-040
- Nome: Acesso sem autenticação
- Módulo: Autenticação (Login)
- Tipo de teste: Funcional / Negativo

---

## Objetivo
- Validar se o sistema impede acesso direto a páginas protegidas sem autenticação prévia.
---

## Ambiente de Teste
- Aplicação: SauceDemo
- URL: https://www.saucedemo.com/
- Navegador: Google Chrome
- Modo de execução: Aba anônima (Incognito)
- Sistema operacional: Windows 11
- Dados utilizados:
  - URL: https://www.saucedemo.com/inventory.html

---

## Passos executados
1. Abrir nova aba anônima.
2. Não realizar autenticação
3. Acessar diretamente::
   "https://www.saucedemo.com/inventory.html".
---

## Resultado obtido

- O sistema bloqueou corretamente o acesso direto à rota protegida e redirecionou o usuário para a tela de login ao identificar ausência de sessão autenticada.

"Epic sadface: You can only access '/inventory.html' when you are logged in"

O sistema destacou o erro visualmente utilizando borda vermelha e ícones de validação.

---

## Resultado esperado
- O sistema deve impedir acesso à página protegida sem autenticação e redirecionar o usuário para a tela de login com mensagem apropriada.
---

## Status do teste
✔ PASSOU

---

## Evidência
- Print disponível em:
  evidences/ct-040-acesso-sem-autenticação.png

---
## Observações
O sistema apresentou comportamento adequado de proteção de rota, impedindo acesso não autenticado à página inventory.html. Não foram identificados vazamentos visuais, exposição de conteúdo interno ou falhas de redirecionamento.
---

## Responsável
Wesllem S. Campos
