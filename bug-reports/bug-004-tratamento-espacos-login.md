# BUG-004 - Login não trata espaços extras no campo de usuário

---

## Tipo
Melhoria de UX / Usabilidade

---

## Resumo
O sistema não remove automaticamente espaços em branco inseridos antes ou depois do nome de usuário, resultando em falha de autenticação mesmo quando as credenciais principais estão corretas.

---

## Ambiente
- Aplicação: SauceDemo
- Navegador: Google Chrome
- Sistema Operacional: Windows 11
- Modo de execução: Aba anônima

---

## 🧪 Cenários relacionados
- CT-005 — Espaços antes do usuário
- CT-006 — Espaços depois do usuário
  
---

## 🧪 Passos para reproduzir

### Cenário 1 — Espaços antes do usuário
1. Acessar a página de login
2. Inserir:
   "  standard_user"
3. Inserir senha válida
4. Clicar no botão Login

---

### Cenário 2 — Espaços depois do usuário
1. Acessar a página de login
2. Inserir:
   "standard_user  "
3. Inserir senha válida
4. Clicar no botão Login

---

## Resultado atual
Sistema bloqueia autenticação e exibe mensagem genérica de erro:

"Epic sadface: Username and password do not match any user in this service"

---

## Resultado esperado
Sistema bloqueia autenticação e apresenta mensagem genérica de erro ao detectar espaços extras no campo de usuário.

---

## Severidade
Baixa

---

## Prioridade
Baixa

---

## Impacto
O comportamento não compromete a segurança ou funcionalidade da aplicação, porém pode causar falhas involuntárias de autenticação e impactar negativamente a experiência do usuário.

## Evidência
evidences/ct-005-negat-espaço-antes-usuario.png
evidences/ct-006-negat-espaço-depois-usuario.png

---

## Reportado por
Wesllem S. Campos
