# Casos de Teste - Login

## Validação de Campos
| ID | Tipo | Cenário | Passos | Resultado Esperado |
|----|------|----------|---------|-------------------|
| CT-001 | POSIT | Login válido | Inserir usuário válido e senha válida | Usuário acessa o sistema |
| CT-002 | NEGAT | Senha inválida | Inserir senha incorreta | Sistema exibe mensagem de erro |
| CT-003 | NEGAT | Usuário inválido | Inserir usuário inexistente | Sistema exibe mensagem de erro |
| CT-004 | NEGAT | Usuário inexistente | Inserir usuário não cadastrado | Sistema exibe mensagem de usuário inválido |
| CT-005 | NEGAT | Espaços antes do Usuário | Inserir espaços antes do  Usuário | Sistema remove espaços ou valida corretamente |
| CT-006 | NEGAT | Espaços depois do Usuário| Inserir espaços após o Usuário | Sistema remove espaços ou valida corretamente |
| CT-007 | NEGAT | Letras maiúsculas no  Usuário | Inserir letras maiúsculas  suário | Sistema deve validar conforme regra de case sensitivity |
| CT-008 | POSIT | Campo senha mascarado | Digitar senha no campo senha | Caracteres devem aparecer mascarados |
| CT-009 | NEGAT | Limite mínimo da senha | Inserir senha abaixo do mínimo | Sistema exibe validação |
| CT-010 | NEGAT | Limite máximo da senha | Inserir senha muito longa | Sistema limita ou valida entrada |
| CT-011 | NEGAT | Caracteres especiais no login | Inserir caracteres especiais inválidos | Sistema trata entrada corretamente |
| CT-012 | POSIT | Copiar e colar senha | Copiar senha e colar no campo | Sistema aceita preenchimento corretamente |
| CT-013 | NEGAT | Campos obrigatórios vazios | Tentar login sem preencher campos | Sistema exibe obrigatoriedade |
| CT-014 | NEGAT | Apenas números no e-mail | Inserir somente números | Sistema valida entrada inválida |
| CT-015 | NEGAT | Apenas letras na senha | Inserir somente letras | Sistema valida conforme regra |
| CT-016 | NEGAT | Emojis nos campos | Inserir emojis nos campos | Sistema trata entrada corretamente |
| CT-017 | POSIT | Caracteres acentuados | Inserir caracteres acentuados | Sistema valida corretamente |
| CT-018 | NEGAT | Sensibilidade da senha | Inserir senha com caixa diferente | Sistema diferencia maiúsculas e minúsculas |
| CT-019 | POSIT | Persistência após erro | Corrigir dados após erro de login | Dados válidos permanecem preenchidos |

---

## Mensagens e Feedback
| ID | Tipo | Cenário | Passos | Resultado Esperado |
|----|------|----------|---------|-------------------|
| CT-020 | POSIT | Exibição da mensagem de erro | Inserir senha inválida | Sistema exibe mensagem de erro |
| CT-021 | POSIT | Remoção da mensagem após nova tentativa | Corrigir login após erro | Mensagem anterior desaparece |
| CT-022 | POSIT | Idioma das mensagens | Executar fluxo inválido | Mensagens devem estar em português |
| CT-023 | NEGAT | Campo senha vazio | Tentar login sem senha | Sistema exibe obrigatoriedade |
| CT-024 | NEGAT | Campo e-mail vazio | Tentar login sem e-mail | Sistema exibe obrigatoriedade |
| CT-025 | NEGAT | Usuário inexistente | Inserir usuário inválido | Sistema exibe mensagem apropriada |
| CT-026 | NEGAT | Senha incorreta | Inserir senha incorreta | Sistema exibe mensagem apropriada |
| CT-027 | NEGAT | Campos obrigatórios | Deixar campos vazios | Sistema informa obrigatoriedade |
| CT-028 | POSIT | Padronização visual | Executar mensagens de erro | Mensagens seguem padrão visual |
| CT-029 | POSIT | Tempo de exibição | Gerar mensagem de erro | Mensagem permanece tempo adequado |
| CT-030 | POSIT | Mensagens em mobile | Executar erro em mobile | Mensagem permanece visível |
| CT-031 | NEGAT | Sobreposição de elementos | Gerar múltiplas mensagens | Interface não deve quebrar |
| CT-032 | POSIT | Clareza da mensagem | Executar fluxo inválido | Mensagem deve ser compreensível |
| CT-033 | NEGAT | Múltiplas tentativas inválidas | Errar login várias vezes | Sistema informa bloqueio |
| CT-034 | POSIT | Mensagens em diferentes resoluções | Alterar resolução da tela | Mensagens permanecem legíveis |

---

## Segurança
| ID | Tipo | Cenário | Passos | Resultado Esperado |
|----|------|----------|---------|-------------------|
| CT-035 | NEGAT | Bloqueio após múltiplas tentativas | Inserir senha incorreta várias vezes | Conta deve ser bloqueada temporariamente |
| CT-036 | POSIT | Expiração de sessão | Permanecer inativo | Sistema encerra sessão |
| CT-037 | POSIT | Senha oculta no HTML | Inspecionar campo senha | Campo deve possuir type="password" |
| CT-038 | NEGAT | SQL Injection | Inserir comandos SQL nos campos | Sistema bloqueia tentativa |
| CT-039 | NEGAT | XSS nos campos | Inserir scripts nos campos | Sistema sanitiza entrada |
| CT-040 | NEGAT | Acesso sem autenticação | Acessar URL interna sem login | Sistema redireciona para login |
| CT-041 | POSIT | Logout correto | Realizar logout | Sessão deve ser encerrada |
| CT-042 | NEGAT | Botão voltar após logout | Fazer logout e clicar voltar | Sistema não permite acesso |
| CT-043 | POSIT | Armazenamento seguro da sessão | Validar sessão ativa | Sessão deve estar protegida |
| CT-044 | POSIT | Expiração do token | Permanecer muito tempo logado | Token deve expirar |
| CT-045 | NEGAT | Reutilização da sessão | Fazer logout e reutilizar sessão | Sistema deve invalidar sessão |
| CT-046 | NEGAT | URL direta | Inserir URL protegida manualmente | Sistema exige autenticação |
| CT-047 | NEGAT | Proteção contra brute force | Realizar diversas tentativas | Sistema limita acessos |
| CT-048 | POSIT | Criptografia da senha | Realizar login | Dados devem trafegar protegidos |
| CT-049 | POSIT | Alteração de senha | Alterar senha da conta | Sessão antiga deve ser invalidada |
| CT-050 | POSIT | Login simultâneo | Acessar em múltiplos dispositivos | Sistema deve tratar sessões |
| CT-051 | POSIT | Fechamento do navegador | Fechar navegador logado | Sessão deve encerrar conforme regra |
| CT-052 | POSIT | Redirecionamento seguro | Realizar login | Sistema deve redirecionar corretamente |
| CT-053 | NEGAT | Scripts maliciosos | Inserir scripts nos campos | Sistema bloqueia execução |
| CT-054 | NEGAT | Sessão expirada | Utilizar sessão vencida | Sistema solicita novo login |

---

## Usabilidade
| ID | Tipo | Cenário | Passos | Resultado Esperado |
|----|------|----------|---------|-------------------|
| CT-055 | POSIT | Navegação utilizando tecla TAB | Navegar pelos campos usando TAB | Foco deve seguir ordem correta |
| CT-056 | POSIT | Login pressionando ENTER | Preencher login e pressionar ENTER | Sistema realiza login |
| CT-057 | POSIT | Responsividade em mobile | Abrir tela em dispositivo mobile | Layout deve adaptar corretamente |
| CT-058 | POSIT | Alinhamento dos campos | Acessar tela de login | Campos devem estar alinhados |
| CT-059 | NEGAT | Botão desabilitado com campos vazios | Deixar campos vazios | Botão login deve permanecer desabilitado |
| CT-060 | POSIT | Indicador de carregamento | Realizar login | Sistema exibe loading durante autenticação |
| CT-061 | POSIT | Foco automático no primeiro campo | Abrir tela de login | Cursor deve iniciar no primeiro campo |
| CT-062 | POSIT | Ordem correta de navegação | Navegar utilizando teclado | Ordem de foco deve ser lógica |
| CT-063 | POSIT | Contraste visual dos elementos | Visualizar tela | Elementos devem possuir boa legibilidade |
| CT-064 | POSIT | Legibilidade da fonte | Visualizar textos da tela | Fonte deve ser legível |
| CT-065 | POSIT | Usabilidade em telas menores | Abrir sistema em resolução reduzida | Interface deve permanecer utilizável |
| CT-066 | POSIT | Posicionamento do botão login | Acessar tela de login | Botão deve estar visível e acessível |
| CT-067 | POSIT | Acessibilidade básica | Navegar utilizando teclado | Sistema deve permitir navegação acessível |
| CT-068 | POSIT | Clique utilizando mouse | Interagir com os campos | Campos devem responder corretamente |
| CT-069 | POSIT | Navegação apenas com teclado | Utilizar sistema sem mouse | Fluxo deve funcionar corretamente |
| CT-070 | POSIT | Efeito visual ao passar mouse | Passar cursor sobre botões | Sistema deve apresentar feedback visual |
| CT-071 | POSIT | Consistência visual da tela | Navegar pela interface | Elementos devem manter padrão visual |
| CT-072 | POSIT | Usabilidade com zoom | Aplicar zoom na página | Interface deve continuar funcional |
| CT-073 | POSIT | Tempo de resposta visual | Interagir com botões | Interface deve responder rapidamente |
| CT-074 | POSIT | Rotação de tela mobile | Alternar orientação do dispositivo | Layout deve adaptar corretamente |

---

## Performance
| ID | Tipo | Cenário | Passos | Resultado Esperado |
|----|------|----------|---------|-------------------|
| CT-075 | POSIT | Carregamento da tela | Abrir tela de login | Tela deve carregar rapidamente |
| CT-076 | POSIT | Tempo de resposta do login | Realizar login | Sistema responde dentro do esperado |
| CT-077 | POSIT | Múltiplas tentativas consecutivas | Realizar vários logins seguidos | Sistema mantém estabilidade |
| CT-078 | POSIT | Internet lenta | Realizar login em conexão lenta | Sistema continua funcional |
| CT-079 | POSIT | Mobile com conexão reduzida | Acessar via mobile | Sistema mantém desempenho aceitável |
| CT-080 | POSIT | Alto volume de acessos | Simular múltiplos usuários | Sistema permanece estável |
| CT-081 | POSIT | Consumo de memória | Utilizar sistema continuamente | Consumo deve permanecer controlado |
| CT-082 | POSIT | Travamentos na autenticação | Executar login repetidamente | Sistema não deve travar |
| CT-083 | NEGAT | Atualização durante login | Atualizar página durante autenticação | Sistema trata ação corretamente |
| CT-084 | POSIT | Tempo de logout | Realizar logout | Logout deve ocorrer rapidamente |
| CT-085 | POSIT | Recuperação de senha | Solicitar recuperação | Sistema responde rapidamente |
| CT-086 | POSIT | Carga simultânea | Simular acessos simultâneos | Sistema suporta carga |
| CT-087 | POSIT | Múltiplas abas abertas | Abrir várias abas logadas | Sistema mantém estabilidade |
| CT-088 | POSIT | Navegadores diferentes | Executar login em vários navegadores | Sistema mantém desempenho |
| CT-089 | POSIT | Mensagens de erro | Gerar mensagens de erro | Mensagens carregam rapidamente |
| CT-090 | POSIT | Longo período de uso | Utilizar sistema por hours | Sistema permanece estável |
| CT-091 | NEGAT | Conexão intermitente | Oscilar conexão durante login | Sistema trata reconexão |
| CT-092 | POSIT | Redirecionamento após login | Realizar login | Redirecionamento ocorre rapidamente |
| CT-093 | POSIT | Impacto do cache | Reabrir sistema utilizando cache | Sistema mantém funcionamento |
| CT-094 | POSIT | Dispositivos antigos | Executar sistema em hardware antigo | Sistema continua utilizável |

---

## Compatibilidade
| ID | Tipo | Cenário | Passos | Resultado Esperado |
|----|------|----------|---------|-------------------|
| CT-095 | POSIT | Login no Google Chrome | Realizar login no Chrome | Sistema funciona corretamente |
| CT-096 | POSIT | Login no Mozilla Firefox | Realizar login no Firefox | Sistema funciona corretamente |
| CT-097 | POSIT | Login no Microsoft Edge | Realizar login no Edge | Sistema funciona corretamente |
| CT-098 | POSIT | Login no Opera | Realizar login no Opera | Sistema funciona corretamente |
| CT-099 | POSIT | Login no Safari | Realizar login no Safari | Sistema funciona corretamente |
| CT-100 | POSIT | Funcionamento em Android | Acessar sistema em Android | Sistema funciona corretamente |
| CT-101 | POSIT | Funcionamento em iPhone | Acessar sistema em iPhone | Sistema funciona corretamente |
| CT-102 | POSIT | Funcionamento em tablet | Acessar sistema em tablet | Sistema adapta interface |
| CT-103 | POSIT | Funcionamento em Windows | Executar sistema no Windows | Sistema funciona corretamente |
| CT-104 | POSIT | Funcionamento em Linux | Executar sistema no Linux | Sistema funciona corretamente |
| CT-105 | POSIT | Diferentes resoluções | Alterar resolução da tela | Interface adapta corretamente |
| CT-106 | POSIT | Modo paisagem mobile | Rotacionar dispositivo | Sistema adapta layout |
| CT-107 | POSIT | Modo retrato mobile | Utilizar dispositivo na vertical | Sistema mantém usabilidade |
| CT-108 | POSIT | Diferentes versões do navegador | Testar versões distintas | Sistema mantém compatibilidade |
| CT-109 | POSIT | Zoom do navegador | Aplicar zoom na página | Sistema permanece funcional |
| CT-110 | POSIT | Tema escuro do sistema | Ativar dark mode do SO | Interface permanece legível |
| CT-111 | POSIT | Diferentes tamanhos de tela | Alterar tamanho da janela | Sistema adapta layout |
| CT-112 | POSIT | Monitores ultrawide | Abrir sistema em ultrawide | Interface permanece alinhada |
| CT-113 | POSIT | Teclado virtual mobile | Abrir teclado em mobile | Campos permanecem acessíveis |
| CT-114 | POSIT | Sistemas operacionais distintos | Alternar entre sistemas | Sistema mantém funcionamento |

---

## Sessão
| ID | Tipo | Cenário | Passos | Resultado Esperado |
|----|------|----------|---------|-------------------|
| CT-115 | POSIT | Atualizar página logado | Atualizar página após login | Sessão permanece ativa |
| CT-116 | POSIT | Fechar navegador | Fechar navegador logado | Sessão encerra conforme regra |
| CT-117 | POSIT | Login simultâneo | Logar em múltiplos dispositivos | Sistema treats sessões corretamente |
| CT-118 | POSIT | Timeout da sessão | Permanecer inativo | Sessão expira corretamente |
| CT-119 | NEGAT | Redirecionamento após expiração | Utilizar sessão expirada | Sistema retorna ao login |
| CT-120 | POSIT | Renovação automática da sessão | Permanecer ativo no sistema | Sessão é renovada |
| CT-121 | POSIT | Logout correto | Executar logout | Sessão é encerrada |
| CT-122 | POSIT | Sessão em múltiplas abas | Abrir várias abas | Sessão permanece consistente |
| CT-123 | NEGAT | Sessão inválida | Utilizar sessão inválida | Sistema solicita autenticação |
| CT-124 | NEGAT | Perda de conexão | Perder conexão durante sessão | Sistema trata reconexão |

---

## Recuperação de Senha
| ID | Tipo | Cenário | Passos | Resultado Esperado |
|----|------|----------|---------|-------------------|
| CT-125 | POSIT | Link “Esqueci minha senha” | Clicar no link | Sistema abre fluxo de recuperação |
| CT-126 | POSIT | Recuperação com e-mail válido | Inserir e-mail válido | Sistema envia recuperação |
| CT-127 | NEGAT | Recuperação com e-mail inválido | Inserir e-mail inválido | Sistema exibe mensagem de erro |
| CT-128 | POSIT | Recebimento do e-mail | Solicitar recuperação | Usuário recebe e-mail |
| CT-129 | NEGAT | Expiração do link | Utilizar link expirado | Sistema informa expiração |
| CT-130 | NEGAT | Reutilização do link | Reutilizar link antigo | Sistema bloqueia reutilização |
| CT-131 | POSIT | Nova senha válida | Inserir senha válida | Senha é redefinida |
| CT-132 | NEGAT | Senha fora do padrão | Inserir senha inválida | Sistema valida regra |
| CT-133 | NEGAT | Confirmação de senha | Inserir confirmação incorreta | Sistema exibe erro |
| CT-134 | POSIT | Mensagem de sucesso | Finalizar redefinição | Sistema informa sucesso |
