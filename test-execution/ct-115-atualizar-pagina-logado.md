# Relatório de Execução de Teste - CT-115

## Identificação do Teste
- ID: CT-115
- Nome: Atualizar página logado
- Módulo: Autenticação (Login)
- Tipo de teste: Funcional / Positivo

---

## Objetivo
- Validar se a sessão do usuário permanece ativa após a atualização da página.
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
4. Clicar no botão Login.
5. Confirmar acesso à página de produtos.
6. Atualizar a página utilizando F5 ou o botão de atualização do navegador.

## Resultado obtido
- O sistema validou corretamente as credenciais informadas e realizou a autenticação com sucesso.

- Após a atualização da página, o usuário permaneceu autenticado e continuou com acesso à página de produtos (inventory.html).

- Não foram observadas mensagens de erro, perda de sessão ou redirecionamentos indevidos.


---

## Resultado esperado
- Usuário deve realizar login com sucesso
- Sistema deve redirecionar para a página de produtos
- A sessão deve permanecer ativa após a atualização da página.
---

## Status do teste
✔ PASSOU

---


## Evidência
- Print disponível em:
  evidences/ct-115-login-enter.png
  
---

## Observações
- O teste demonstrou que a aplicação mantém corretamente a sessão autenticada após atualização da página, garantindo continuidade da navegação sem necessidade de novo login. Garantindo uma boa experiência para o usuário.


## Responsável
Wesllem S. Campos
