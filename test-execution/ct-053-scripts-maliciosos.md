# Relatório de Execução de Teste - CT-053

## Identificação do Teste
- ID: CT-053
- Nome: Scripts maliciosos
- Módulo: Autenticação (Login)
- Tipo de teste: Funcional / Negativo

---

## Objetivo
- Validar se o sistema trata corretamente entradas contendo scripts e impede sua execução.

---

## Ambiente de Teste
- Aplicação: SauceDemo
- URL: https://www.saucedemo.com/
- Navegador: Google Chrome
- Modo de execução: Aba anônima (Incognito)
- Sistema operacional: Windows 11

---

### Payload 1
Usuário:
<script>alert('XSS')</script>

Senha:
123

---

### Payload 2
Usuário:
<img src=x onerror=alert('XSS')>

Senha:
123

---

### Payload 3
Usuário:
<svg onload=alert('XSS')>

Senha:
123

---

## Passos executados
1. Acessar página de login
2. Inserir payload XSS nos campos
3. Clicar no botão Login.

---

## Resultado obtido
O sistema bloqueou corretamente a autenticação para todos os payloads testados.

A aplicação apresentou mensagem genérica de erro:

"Epic sadface: Username and password do not match any user in this service".

Não foram identificados:
- erros SQL.
- exposição de stack trace.
- falhas visuais.
- comportamento inesperado.

A URL permaneceu na tela de login.
Não foram identificadas execuções de JavaScript, exibição de alertas, alterações inesperadas na interface ou qualquer indício de interpretação dos payloads enviados.

---

## Resultado esperado
Sistema deve tratar entradas scripts como texto comum, impedindo autenticação indevida e evitando exposição de informações internas.

## Status do teste
✔ PASSOU

---

## Evidência
- Print disponível em:
  evidences/ct-053-xss-script.png

  evidences/ct-053-xss-img.png

  evidences/ct-053-xss-svg.png
  
---

## Observações
- O teste demonstrou que a aplicação possui mecanismos básicos de proteção contra execução de scripts injetados nos campos de autenticação, reduzindo riscos relacionados a ataques do tipo Cross-Site Scripting (XSS).

## Responsável
Wesllem S. Campos
