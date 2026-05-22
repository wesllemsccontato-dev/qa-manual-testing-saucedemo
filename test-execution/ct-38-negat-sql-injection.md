# Relatório de Execução de Teste - CT-038

## Identificação do Teste
- ID: CT-038
- Nome: SQL Injection
- Módulo: Autenticação (Login)
- Tipo de teste: Segurança / Negativo

---

## Objetivo
Validar se o sistema bloqueia tentativas de autenticação utilizando comandos SQL nos campos de login.

---

## Ambiente de Teste
- Aplicação: SauceDemo
- URL: https://www.saucedemo.com/
- Navegador: Google Chrome
- Sistema operacional: Windows 11
- Modo de execução: Aba anônima

---

## Payloads utilizados

### Payload 1
Usuário:
' OR '1'='1

Senha:
' OR '1'='1

---

### Payload 2
Usuário:
admin' --

Senha:
123

---

## Passos executados
1. Acessar página de login
2. Inserir payload SQL nos campos
3. Clicar no botão Login

---

## Resultado obtido
O sistema bloqueou autenticação corretamente para ambos os cenários testados.

A aplicação apresentou mensagem genérica de erro:

"Epic sadface: Username and password do not match any user in this service"

Não foram identificados:
- erros SQL
- exposição de stack trace
- falhas visuais
- comportamento inesperado

A URL permaneceu na tela de login.

---

## Resultado esperado
Sistema deve tratar entradas SQL como texto comum, impedindo autenticação indevida e evitando exposição de informações internas.

---

## Status do teste
✔ PASSOU

---

## Observações
A utilização de mensagem genérica contribui positivamente para segurança da autenticação, reduzindo exposição de informações sobre usuários válidos ou inválidos.

---

## Evidências
- evidences/ct-038-negat-sql-1-injection.png
- evidences/ct-038-negat-sql-2-injection.png

---

## Responsável
Wesllem S. Campos
