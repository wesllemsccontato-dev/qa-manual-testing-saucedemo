# BUG-005 - Ausência de aviso visual para Caps Lock ativado no login

---

## Tipo
Melhoria de UX / Usabilidade

---

## Resumo
O sistema apresentou comportamento funcional esperado ao bloquear autenticação com diferença de caixa no nome de usuário. Entretanto, a mensagem genérica pode dificultar a identificação da causa real do erro pelo usuário final, impactando a experiência de autenticação.

---

## Ambiente
- Aplicação: SauceDemo
- Navegador: Google Chrome
- Sistema Operacional: Windows 11
- Modo de execução: Aba anônima

---

## Cenários relacionados
- CT-007 — Usuário em letras maiúsculas

---

## Passos para reproduzir
1. Ativar a tecla Caps Lock
2. Acessar a página de login
3. Inserir usuário em letras maiúsculas:
   "STANDARD_USER"
4. Inserir senha válida
5. Clicar no botão Login

---


## Resultado atual
Sistema bloqueia autenticação e exibe mensagem genérica de erro:

"Epic sadface: Username and password do not match any user in this service".

Sem informar ao usuário que o Caps Lock pode estar ativado.

---

## Resultado esperado
Sistema deve apresentar aviso visual indicando que a tecla Caps Lock está ativada durante o preenchimento dos campos de autenticação.

---

## Severidade
Baixa

---

## Prioridade
Baixa

---

## Impacto
O comportamento não afeta diretamente a funcionalidade ou segurança da aplicação, porém pode gerar erros involuntários de autenticação e dificultar a identificação da causa do problema pelo usuário final.


## Sugestão de melhoria
Adicionar indicador visual de Caps Lock ativado próximo aos campos de login e senha para auxiliar o usuário durante autenticação.



## Evidência
evidences/ct-007-negat-usuario-em-maiusculo.png

---

## Reportado por
Wesllem S. Campos
