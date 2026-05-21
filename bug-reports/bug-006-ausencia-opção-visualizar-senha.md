# BUG-006 - Ausência de opção para visualizar senha durante autenticação

---

## Tipo
Melhoria de UX / Usabilidade

---

## Resumo
- O sistema apresentou comportamento funcional esperado ao mascarar a senha digitada. Entretanto, a ausecia de disponibilidade de desabilitar/abilitar essa função pode dificultar a identificação do que esta sendo ditado pelo usuário final, impactando a experiência de autenticação.

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
1. Acessar a página de login.
2. Localizar campo Password
3. Inserir senha válida:
"secret_sauce".


---


## Resultado atual
- Sistema mascara corretamente todos os caracteres digitados no campo de senha.


---

## Resultado esperado
- Sistema deve oferecer mecanismo opcional para visualização da senha digitada, auxiliando o usuário durante autenticação.


---

## Severidade
Baixa

---

## Prioridade
Baixa

---

## Impacto
- O comportamento não afeta diretamente segurança da aplicação, porém pode gerar erros involuntários de autenticação e dificultar a identificação da causa do problema pelo usuário final.


## Sugestão de melhoria
- Adicionar botão de “mostrar/ocultar senha” próximo ao campo de senha para permitir visualização temporária do conteúdo digitado durante autenticação.


## Evidência
evidences/ct-008-posit-campo-senha-mascarado.png

---

## Reportado por
Wesllem S. Campos
