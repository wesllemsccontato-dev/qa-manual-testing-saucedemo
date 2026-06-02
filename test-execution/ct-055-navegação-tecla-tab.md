# Relatório de Execução de Teste - CT-055

## Identificação do Teste
- ID: CT-055
- Nome: Navegação utilizando tecla TAB
- Módulo: Autenticação (Login)
- Tipo de teste: Funcional / Positivo

---

## Objetivo
- Validar se o sistema permite a navegação pela tecla TAB, seguindo uma ordem lógica entre os elementos da interface.
---

## Ambiente de Teste
- Aplicação: SauceDemo
- URL: https://www.saucedemo.com/
- Navegador: Google Chrome
- Modo de execução: Aba anônima (Incognito)
- Sistema operacional: Windows 11

---

## Passos executados
1. Acessar a página de login.
2. Clicar na pagina (Para  garantir o foco)
3. Pressione TAB repetidamente.
4. Observar a ordem de navegação entre os elementos da tela

## Resultado obtido

- O sistema seguiu corretamente a ordem esperada de navegação, permitindo a movimentação do foco entre os campos Username, Password e o botão Login utilizando apenas a tecla TAB.

Foi possível navegar pela interface sem utilização do mouse.

---

## Resultado esperado
- O foco deve seguir uma ordem lógica entre os elementos da interface, permitindo navegação completa através do teclado.
---

## Status do teste
✔ PASSOU

---

## Critérios de acessibilidade avaliados
- Navegação por teclado
- Ordem lógica do foco
- Visibilidade do foco
- Operação sem uso do mouse

## Evidência
- Print disponível em:
  evidences/ct-055-tab-username.png

  evidences/ct-055-tab-password.png

  evidences/ct-055-tab-login.png
  
---

## Observações
- A funcionalidade de navegação por teclado apresentou comportamento correto e permitiu utilização da tela sem mouse.

- Entretanto, foi observado que o botão Login não apresenta indicação visual suficientemente clara quando recebe foco por navegação via teclado, cenário relacionado ao BUG-007.

---

## Responsável
Wesllem S. Campos
