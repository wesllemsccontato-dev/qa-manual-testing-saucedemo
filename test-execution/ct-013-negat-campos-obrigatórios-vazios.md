# Relatório de Execução de Teste - CT-013

## Identificação do Teste
- ID: CT-013
- Nome: Campos obrigatórios vazios
- Módulo: Autenticação (Login)
- Tipo de teste: Funcional / Negativo

---

## Objetivo
- Validar comportamento do sistema ao tentar autenticação sem preenchimento dos campos obrigatórios.

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
2. Manter os campos usuario e senha vazios.
3. Clicar no botão Login

---

## Resultado obtido
- Sistema bloqueou autenticação corretamente e apresentou mensagem:

"Epic sadface: Username is required"

O sistema destacou visualmente o campo inválido utilizando borda vermelha e ícones de erro.

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
  evidences/ct-013-negat-campos-obrigatorios-vazios.png

---

## Observações
- O botão Login permaneceu habilitado mesmo com campos vazios.
- O sistema priorizou validação do primeiro campo obrigatório.
- Layout e feedback visual permaneceram consistentes.

---

## Responsável
Wesllem S. Campos
