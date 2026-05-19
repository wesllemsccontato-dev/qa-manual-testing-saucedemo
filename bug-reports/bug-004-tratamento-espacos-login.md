# BUG-004 - Login não ignora espaços antes do nome de usuário

---

## Tipo
Melhoria de UX / Usabilidade

---

## Resumo
O sistema não remove automaticamente espaços em branco inseridos antes do nome de usuário, resultando em falha de autenticação mesmo quando as credenciais principais estão corretas.

---

## Ambiente
- Aplicação: SauceDemo
- Navegador: Google Chrome
- Sistema Operacional: Windows 11
- Modo de execução: Aba anônima

---

## Passos para reproduzir
1. Acessar a página de login
2. Inserir espaços antes do usuário:
   "  standard_user"
3. Inserir senha valida
4. Clicar no botão Login

---

## Resultado atual
Sistema bloqueia autenticação e exibe mensagem genérica de erro:

"Epic sadface: Username and password do not match any user in this service"

---

## Resultado esperado
Sistema pode remover automaticamente espaços desnecessários antes do nome de usuário ou apresentar validação mais clara ao usuário.

---

## Severidade
Baixa

---

## Prioridade
Baixa

---

## Impacto
O comportamento não afeta diretamente a segurança ou funcionamento da aplicação, porém pode gerar falhas de autenticação involuntárias e impactar a experiência do usuário.

## Evidência
evidences/ct-005-negat-espaço-antes-usuario.png

---

## Reportado por
Wesllem S. Campos
