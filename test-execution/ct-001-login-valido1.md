# Relatório de Execução de Teste - CT-001

## Identificação do Teste
- ID: CT-001
- Nome: Login válido
- Módulo: Autenticação (Login)
- Tipo de teste: Funcional / Positivo

---

## Objetivo
Validar que o usuário consegue realizar login com credenciais válidas no sistema SauceDemo.

---

## Ambiente de Teste
- Aplicação: SauceDemo
- URL: https://www.saucedemo.com/
- Navegador: Google Chrome
- Modo de execução: Aba anônima (Incognito)
- Sistema operacional: Windows 11
- Dados utilizados:
  - Usuário: standard_user
  - Senha: secret_sauce

---

## Passos executados
1. Acessar a página de login
2. Inserir usuário válido (standard_user)
3. Inserir senha válida (secret_sauce)
4. Clicar no botão "Login"

---

## Resultado obtido
- Usuário foi redirecionado com sucesso para a página de inventário
- URL exibida: https://www.saucedemo.com/inventory.html
- Lista de produtos carregada corretamente na tela

---

## Resultado esperado
- Usuário deve realizar login com sucesso
- Sistema deve redirecionar para a página de produtos

---

## Status do teste
✔ PASSOU

---

## Evidência
Print disponível em:
evidences/ct-001-login-success.png

## 🧠 Observações
O sistema apresentou comportamento esperado...

## 👤 Responsável
Wesllem S. Campos
