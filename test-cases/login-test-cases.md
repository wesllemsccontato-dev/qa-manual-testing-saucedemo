# Casos de Teste - Login

Validação de Campos
| ID | Cenário | Passos | Resultado Esperado |
|----|----------|---------|-------------------|
| CT-001 | Login válido | Inserir usuário válido e senha válida | Usuário acessa o sistema |
| CT-002 | Senha inválida | Inserir senha incorreta | Sistema exibe mensagem de erro |
| CT-003 | E-mail inválido sem @ | Inserir e-mail sem @ | Sistema valida formato inválido |
| CT-004 | E-mail inexistente | Inserir e-mail não cadastrado | Sistema exibe mensagem de usuário inválido |
| CT-005 | Espaços antes do e-mail | Inserir espaços antes do e-mail | Sistema remove espaços ou valida corretamente |
| CT-006 | Espaços depois do e-mail | Inserir espaços após o e-mail | Sistema remove espaços ou valida corretamente |
| CT-007 | Letras maiúsculas no e-mail | Inserir e-mail em maiúsculo | Sistema realiza login corretamente |
| CT-008 | Campo senha mascarado | Digitar senha no campo senha | Caracteres devem aparecer mascarados |
| CT-009 | Limite mínimo da senha | Inserir senha abaixo do mínimo | Sistema exibe validação |
| CT-010 | Limite máximo da senha | Inserir senha muito longa | Sistema limita ou valida entrada |
| CT-011 | Caracteres especiais no login | Inserir caracteres especiais inválidos | Sistema trata entrada corretamente |
| CT-012 | Copiar e colar senha | Copiar senha e colar no campo | Sistema aceita preenchimento corretamente |
| CT-013 | Campos obrigatórios vazios | Tentar login sem preencher campos | Sistema exibe obrigatoriedade |
| CT-014 | Apenas números no e-mail | Inserir somente números | Sistema valida entrada inválida |
| CT-015 | Apenas letras na senha | Inserir somente letras | Sistema valida conforme regra |
| CT-016 | Emojis nos campos | Inserir emojis nos campos | Sistema trata entrada corretamente |
| CT-017 | Caracteres acentuados | Inserir caracteres acentuados | Sistema valida corretamente |
| CT-018 | Sensibilidade da senha | Inserir senha com caixa diferente | Sistema diferencia maiúsculas e minúsculas |
| CT-019 | Persistência após erro | Corrigir dados após erro de login | Dados válidos permanecem preenchidos |

---

Mensagens e Feedback
| ID | Cenário | Passos | Resultado Esperado |
|----|----------|---------|-------------------|
| CT-020 | Exibição da mensagem de erro | Inserir senha inválida | Sistema exibe mensagem de erro |
| CT-021 | Remoção da mensagem após nova tentativa | Corrigir login após erro | Mensagem anterior desaparece |
| CT-022 | Idioma das mensagens | Executar fluxo inválido | Mensagens devem estar em português |
| CT-023 | Campo senha vazio | Tentar login sem senha | Sistema exibe obrigatoriedade |
| CT-024 | Campo e-mail vazio | Tentar login sem e-mail | Sistema exibe obrigatoriedade |
| CT-025 | Usuário inexistente | Inserir usuário inválido | Sistema exibe mensagem apropriada |
| CT-026 | Senha incorreta | Inserir senha incorreta | Sistema exibe mensagem apropriada |
| CT-027 | Campos obrigatórios | Deixar campos vazios | Sistema informa obrigatoriedade |
| CT-028 | Padronização visual | Executar mensagens de erro | Mensagens seguem padrão visual |
| CT-029 | Tempo de exibição | Gerar mensagem de erro | Mensagem permanece tempo adequado |
| CT-030 | Mensagens em mobile | Executar erro em mobile | Mensagem permanece visível |
| CT-031 | Sobreposição de elementos | Gerar múltiplas mensagens | Interface não deve quebrar |
| CT-032 | Clareza da mensagem | Executar fluxo inválido | Mensagem deve ser compreensível |
| CT-033 | Múltiplas tentativas inválidas | Errar login várias vezes | Sistema informa bloqueio |
| CT-034 | Mensagens em diferentes resoluções | Alterar resolução da tela | Mensagens permanecem legíveis |

---

Segurança
| ID | Cenário | Passos | Resultado Esperado |
|----|----------|---------|-------------------|
| CT-035 | Bloqueio após múltiplas tentativas | Inserir senha incorreta várias vezes | Conta deve ser bloqueada temporariamente |
| CT-036 | Expiração de sessão | Permanecer inativo | Sistema encerra sessão |
| CT-037 | Senha oculta no HTML | Inspecionar campo senha | Campo deve possuir type="password" |
| CT-038 | SQL Injection | Inserir comandos SQL nos campos | Sistema bloqueia tentativa |
| CT-039 | XSS nos campos | Inserir scripts nos campos | Sistema sanitiza entrada |
| CT-040 | Acesso sem autenticação | Acessar URL interna sem login | Sistema redireciona para login |
| CT-041 | Logout correto | Realizar logout | Sessão deve ser encerrada |
| CT-042 | Botão voltar após logout | Fazer logout e clicar voltar | Sistema não permite acesso |
| CT-043 | Armazenamento seguro da sessão | Validar sessão ativa | Sessão deve estar protegida |
| CT-044 | Expiração do token | Permanecer muito tempo logado | Token deve expirar |
| CT-045 | Reutilização da sessão | Fazer logout e reutilizar sessão | Sistema deve invalidar sessão |
| CT-046 | URL direta | Inserir URL protegida manualmente | Sistema exige autenticação |
| CT-047 | Proteção contra brute force | Realizar diversas tentativas | Sistema limita acessos |
| CT-048 | Criptografia da senha | Realizar login | Dados devem trafegar protegidos |
| CT-049 | Alteração de senha | Alterar senha da conta | Sessão antiga deve ser invalidada |
| CT-050 | Login simultâneo | Acessar em múltiplos dispositivos | Sistema deve tratar sessões |
| CT-051 | Fechamento do navegador | Fechar navegador logado | Sessão deve encerrar conforme regra |
| CT-052 | Redirecionamento seguro | Realizar login | Sistema deve redirecionar corretamente |
| CT-053 | Scripts maliciosos | Inserir scripts nos campos | Sistema bloqueia execução |
| CT-054 | Sessão expirada | Utilizar sessão vencida | Sistema solicita novo login |

---

Usabilidade
| ID | Cenário | Passos | Resultado Esperado |
|----|----------|---------|-------------------|
| CT-055 | Navegação utilizando tecla TAB | Navegar pelos campos usando TAB | Foco deve seguir ordem correta |
| CT-056 | Login pressionando ENTER | Preencher login e pressionar ENTER | Sistema realiza login |
| CT-057 | Responsividade em mobile | Abrir tela em dispositivo mobile | Layout deve adaptar corretamente |
| CT-058 | Alinhamento dos campos | Acessar tela de login | Campos devem estar alinhados |
| CT-059 | Botão desabilitado com campos vazios | Deixar campos vazios | Botão login deve permanecer desabilitado |
| CT-060 | Indicador de carregamento | Realizar login | Sistema exibe loading durante autenticação |
| CT-061 | Foco automático no primeiro campo | Abrir tela de login | Cursor deve iniciar no primeiro campo |
| CT-062 | Ordem correta de navegação | Navegar utilizando teclado | Ordem de foco deve ser lógica |
| CT-063 | Contraste visual dos elementos | Visualizar tela | Elementos devem possuir boa legibilidade |
| CT-064 | Legibilidade da fonte | Visualizar textos da tela | Fonte deve ser legível |
| CT-065 | Usabilidade em telas menores | Abrir sistema em resolução reduzida | Interface deve permanecer utilizável |
| CT-066 | Posicionamento do botão login | Acessar tela de login | Botão deve estar visível e acessível |
| CT-067 | Acessibilidade básica | Navegar utilizando teclado | Sistema deve permitir navegação acessível |
| CT-068 | Clique utilizando mouse | Interagir com os campos | Campos devem responder corretamente |
| CT-069 | Navegação apenas com teclado | Utilizar sistema sem mouse | Fluxo deve funcionar corretamente |
| CT-070 | Efeito visual ao passar mouse | Passar cursor sobre botões | Sistema deve apresentar feedback visual |
| CT-071 | Consistência visual da tela | Navegar pela interface | Elementos devem manter padrão visual |
| CT-072 | Usabilidade com zoom | Aplicar zoom na página | Interface deve continuar funcional |
| CT-073 | Tempo de resposta visual | Interagir com botões | Interface deve responder rapidamente |
| CT-074 | Rotação de tela mobile | Alternar orientação do dispositivo | Layout deve adaptar corretamente |

---

Performance
| ID | Cenário | Passos | Resultado Esperado |
|----|----------|---------|-------------------|
| CT-075 | Carregamento da tela | Abrir tela de login | Tela deve carregar rapidamente |
| CT-076 | Tempo de resposta do login | Realizar login | Sistema responde dentro do esperado |
| CT-077 | Múltiplas tentativas consecutivas | Realizar vários logins seguidos | Sistema mantém estabilidade |
| CT-078 | Internet lenta | Realizar login em conexão lenta | Sistema continua funcional |
| CT-079 | Mobile com conexão reduzida | Acessar via mobile | Sistema mantém desempenho aceitável |
| CT-080 | Alto volume de acessos | Simular múltiplos usuários | Sistema permanece estável |
| CT-081 | Consumo de memória | Utilizar sistema continuamente | Consumo deve permanecer controlado |
| CT-082 | Travamentos na autenticação | Executar login repetidamente | Sistema não deve travar |
| CT-083 | Atualização durante login | Atualizar página durante autenticação | Sistema trata ação corretamente |
| CT-084 | Tempo de logout | Realizar logout | Logout deve ocorrer rapidamente |
| CT-085 | Recuperação de senha | Solicitar recuperação | Sistema responde rapidamente |
| CT-086 | Carga simultânea | Simular acessos simultâneos | Sistema suporta carga |
| CT-087 | Múltiplas abas abertas | Abrir várias abas logadas | Sistema mantém estabilidade |
| CT-088 | Navegadores diferentes | Executar login em vários navegadores | Sistema mantém desempenho |
| CT-089 | Mensagens de erro | Gerar mensagens de erro | Mensagens carregam rapidamente |
| CT-090 | Longo período de uso | Utilizar sistema por horas | Sistema permanece estável |
| CT-091 | Conexão intermitente | Oscilar conexão durante login | Sistema trata reconexão |
| CT-092 | Redirecionamento após login | Realizar login | Redirecionamento ocorre rapidamente |
| CT-093 | Impacto do cache | Reabrir sistema utilizando cache | Sistema mantém funcionamento |
| CT-094 | Dispositivos antigos | Executar sistema em hardware antigo | Sistema continua utilizável |

---

Compatibilidade
| ID | Cenário | Passos | Resultado Esperado |
|----|----------|---------|-------------------|
| CT-095 | Login no Google Chrome | Realizar login no Chrome | Sistema funciona corretamente |
| CT-096 | Login no Mozilla Firefox | Realizar login no Firefox | Sistema funciona corretamente |
| CT-097 | Login no Microsoft Edge | Realizar login no Edge | Sistema funciona corretamente |
| CT-098 | Login no Opera | Realizar login no Opera | Sistema funciona corretamente |
| CT-099 | Login no Safari | Realizar login no Safari | Sistema funciona corretamente |
| CT-100 | Funcionamento em Android | Acessar sistema em Android | Sistema funciona corretamente |
| CT-101 | Funcionamento em iPhone | Acessar sistema em iPhone | Sistema funciona corretamente |
| CT-102 | Funcionamento em tablet | Acessar sistema em tablet | Sistema adapta interface |
| CT-103 | Funcionamento em Windows | Executar sistema no Windows | Sistema funciona corretamente |
| CT-104 | Funcionamento em Linux | Executar sistema no Linux | Sistema funciona corretamente |
| CT-105 | Diferentes resoluções | Alterar resolução da tela | Interface adapta corretamente |
| CT-106 | Modo paisagem mobile | Rotacionar dispositivo | Sistema adapta layout |
| CT-107 | Modo retrato mobile | Utilizar dispositivo na vertical | Sistema mantém usabilidade |
| CT-108 | Diferentes versões do navegador | Testar versões distintas | Sistema mantém compatibilidade |
| CT-109 | Zoom do navegador | Aplicar zoom na página | Sistema permanece funcional |
| CT-110 | Tema escuro do sistema | Ativar dark mode do SO | Interface permanece legível |
| CT-111 | Diferentes tamanhos de tela | Alterar tamanho da janela | Sistema adapta layout |
| CT-112 | Monitores ultrawide | Abrir sistema em ultrawide | Interface permanece alinhada |
| CT-113 | Teclado virtual mobile | Abrir teclado em mobile | Campos permanecem acessíveis |
| CT-114 | Sistemas operacionais distintos | Alternar entre sistemas | Sistema mantém funcionamento |

---

Sessão
| ID | Cenário | Passos | Resultado Esperado |
|----|----------|---------|-------------------|
| CT-115 | Atualizar página logado | Atualizar página após login | Sessão permanece ativa |
| CT-116 | Fechar navegador | Fechar navegador logado | Sessão encerra conforme regra |
| CT-117 | Login simultâneo | Logar em múltiplos dispositivos | Sistema trata sessões corretamente |
| CT-118 | Timeout da sessão | Permanecer inativo | Sessão expira corretamente |
| CT-119 | Redirecionamento após expiração | Utilizar sessão expirada | Sistema retorna ao login |
| CT-120 | Renovação automática da sessão | Permanecer ativo no sistema | Sessão é renovada |
| CT-121 | Logout correto | Executar logout | Sessão é encerrada |
| CT-122 | Sessão em múltiplas abas | Abrir várias abas | Sessão permanece consistente |
| CT-123 | Sessão inválida | Utilizar sessão inválida | Sistema solicita autenticação |
| CT-124 | Perda de conexão | Perder conexão durante sessão | Sistema trata reconexão |

---

Recuperação de Senha
| ID | Cenário | Passos | Resultado Esperado |
|----|----------|---------|-------------------|
| CT-125 | Link “Esqueci minha senha” | Clicar no link | Sistema abre fluxo de recuperação |
| CT-126 | Recuperação com e-mail válido | Inserir e-mail válido | Sistema envia recuperação |
| CT-127 | Recuperação com e-mail inválido | Inserir e-mail inválido | Sistema exibe mensagem de erro |
| CT-128 | Recebimento do e-mail | Solicitar recuperação | Usuário recebe e-mail |
| CT-129 | Expiração do link | Utilizar link expirado | Sistema informa expiração |
| CT-130 | Reutilização do link | Reutilizar link antigo | Sistema bloqueia reutilização |
| CT-131 | Nova senha válida | Inserir senha válida | Senha é redefinida |
| CT-132 | Senha fora do padrão | Inserir senha inválida | Sistema valida regra |
| CT-133 | Confirmação de senha | Inserir confirmação incorreta | Sistema exibe erro |
| CT-134 | Mensagem de sucesso | Finalizar redefinição | Sistema informa sucesso |
