# BUG-007 - Indicador de foco pouco visível no botão Login durante navegação por teclado

## Tipo
Melhoria de Acessibilidade / UX

## Resumo
Durante navegação utilizando a tecla TAB, o foco dos campos Username e Password pôde ser identificado visualmente. Entretanto, ao chegar no botão Login, não foi possível identificar claramente que o elemento estava selecionado, dificultando a navegação para usuários que utilizam apenas teclado.

## Cenário relacionado
- CT-055 — Navegação utilizando tecla TAB

## Passos para reproduzir
1. Acessar a página de login
2. Navegar utilizando apenas a tecla TAB
3. Observar a indicação visual de foco nos elementos da tela
4. Continuar até o botão Login

## Resultado atual
O botão Login não apresenta indicação visual clara de foco durante navegação por teclado.

## Resultado esperado
O botão Login deve apresentar destaque visual consistente quando receber foco por teclado, permitindo que o usuário identifique facilmente o elemento selecionado.

## Severidade
Baixa

## Prioridade
Baixa

## Impacto
Pode dificultar a navegação para usuários que utilizam teclado como principal meio de interação, reduzindo a acessibilidade da aplicação.

## Evidência
evidences/ct-055-tab-login.png

## Reportado por
Wesllem S. Campos
