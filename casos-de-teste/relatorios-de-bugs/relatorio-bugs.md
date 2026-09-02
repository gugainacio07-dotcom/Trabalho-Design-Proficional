# Relatório de Bugs — Tela de Login

## Formulário permite envio com campos vazios:

**Severidade:** Alta
**Prioridade:** Alta
**Ambiente:** Homologação / Chrome (última versão) / Windows 11

**Descrição:**
Ao clicar em "Entrar" com os campos de e-mail e senha vazios, o sistema não exibe
nenhuma mensagem de validação e realiza uma tentativa de requisição ao servidor,
o que não deveria ocorrer.

**Passos para reproduzir:**
 Acessar a tela de login
 Deixar os campos de e-mail e senha em branco
 Clicar em "Entrar"

**Resultado atual:** Nenhuma mensagem é exibida; a página apenas recarrega
**Resultado esperado:** Sistema deve exibir mensagem "Preencha todos os campos obrigatórios"
e impedir o envio do formulário


**Status:** Aberto


##  Sistema não bloqueia após múltiplas tentativas falhas:

**Severidade:** Média
**Prioridade:** Alta (risco de segurança)
**Ambiente:** Homologação / Chrome (última versão) / Windows 11

**Descrição:**
Após 5 tentativas seguidas de login com senha incorreta, o sistema deveria bloquear
temporariamente novas tentativas (ex: por 5 minutos). No entanto, o sistema continua
aceitando tentativas ilimitadas, o que representa um risco de segurança
(possibilidade de ataque de força bruta).

**Passos para reproduzir:**
 Acessar a tela de login
 Inserir e-mail válido e senha incorreta 5 vezes seguidas
 Observar que o sistema continua aceitando novas tentativas

**Resultado atual:** Sistema permite tentativas ilimitadas de login
**Resultado esperado:** Sistema deve bloquear novas tentativas por um período
determinado após 5 falhas consecutivas


**Status:** Aberto
