# Relatório de Execução de Teste - CT-056

## Identificação do Teste
- ID: CT-056
- Nome: Login pressionando ENTER
- Módulo: Autenticação (Login)
- Tipo de teste: Funcional / Positivo

---

## Objetivo
- Validar se o sistema permite autenticação utilizando a tecla ENTER, sem alternativa  ao clique no botão Login.
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
1. Acessar a página de login.
2. Inserir usuário valido:
   "standard_user".
3. Inserir senha valida:
"secret_sauce".
4. Pressionar a tecla Enter.

## Resultado obtido
- O sistema validou corretamente as credenciais informadas e realizou a autenticação com sucesso após o acionamento da tecla ENTER.

- O usuário foi redirecionado para a página de produtos (inventory.html), sem necessidade de interação com o botão Login.

---

## Resultado esperado
- Usuário deve realizar login com sucesso
- Sistema deve redirecionar para a página de produtos
---

## Status do teste
✔ PASSOU

---


## Evidência
- Print disponível em:
  evidences/ct-056-login-enter.png
  
---

## Observações
- O teste demonstrou que a tecla ENTER executa a mesma ação do botão Login, garantindo uma experiência consistente para usuários que navegam utilizando teclado.


## Responsável
Wesllem S. Campos
