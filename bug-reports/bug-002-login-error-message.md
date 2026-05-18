# BUG-002 - Mensagem de erro com linguagem informal no login inválido

---

## Tipo
Melhoria de UX / Usabilidade

---

## Resumo
A mensagem de erro apresentada no login inválido contém linguagem informal ("Epic sadface"), o que pode impactar a clareza e profissionalismo da comunicação com o usuário.

---

## Ambiente
- Aplicação: SauceDemo
- Navegador: Google Chrome
- Sistema Operacional: Windows 11
- Modo de execução: Aba anônima

---

## Passos para reproduzir
1. Acessar a página de login
2. Inserir usuário válido
3. Inserir senha inválida
4. Clicar no botão Login

---

## Resultado atual
Sistema apresenta a mensagem:

"Epic sadface: Username and password do not match any user in this service"

---

## Resultado esperado
Sistema deve apresentar mensagem de erro mais objetiva e profissional, como:

"Usuário ou senha inválidos"

---

## Severidade
Baixa

---

## Prioridade
Baixa

---

## Impacto
Apesar de não afetar a funcionalidade do sistema, a linguagem utilizada pode reduzir a clareza da comunicação e comprometer a experiência do usuário.

---

## Evidência
evidences/ct-002-invalid-password.png

---

## Reportado por
Wesllem S. Campos
