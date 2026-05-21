# Relatório de Execução de Teste - CT-008

## Identificação do Teste
- ID: CT-008
- Nome: Campo senha mascarado
- Módulo: Autenticação (Login)
- Tipo de teste: Funcional / Positivo

---

## Objetivo
- Validar que o sistema não mostre a senha digitada no campo passord.

---

## Ambiente de Teste
- Aplicação: SauceDemo
- URL: https://www.saucedemo.com/
- Navegador: Google Chrome
- Modo de execução: Aba anônima (Incognito)
- Sistema operacional: Windows 11
- Dados utilizados:
  - Senha: secret_sauce
---

## Passos executados
1. Acessar a página de login.
2. Localizar campo Password
3. Inserir senha válida:
"secret_sauce".

---

## Resultado obtido
- Caracteres do campo Senha  mascarados.

---

## Resultado esperado
- Sistema deve mostar exibir a senha digita 
- Exibir mascara no campo senha.

---

## Status do teste
✔ PASSOU

---

## Evidência
- Print disponível em:
  evidences/ct-008-posit-campo-senha-mascarado.png

---

## Observações
- A aplicação apresentou comportamento esperado ao impedir a vizualização da senha digitada trocando pelo carcter especial "*".

---

## Responsável
Wesllem S. Campos
