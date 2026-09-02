# Casos de Teste — Tela de Login

## Login com credenciais válidas
**Cenário:** Usuário tenta logar com e-mail e senha corretos
**Pré-condição:** Usuário previamente cadastrado no sistema
**Passos:**
Acessar a tela de login:
 Inserir e-mail válido: `usuario@teste.com`
 Inserir senha válida: `Senha123!`
 Clicar em "Entrar"

**Resultado esperado:** Usuário é redirecionado para a tela inicial (dashboard)
**Status:**  Passou


## Login com senha incorreta:
**Cenário:** Usuário tenta logar com e-mail válido, mas senha incorreta
**Pré-condição:** Usuário previamente cadastrado no sistema
**Passos:**
 Acessar a tela de login
 Inserir e-mail válido: `usuario@teste.com`
 Inserir senha inválida: `SenhaErrada`
 Clicar em "Entrar"

**Resultado esperado:** Sistema exibe mensagem "E-mail ou senha inválidos" e não permite o acesso
**Status:**  Passou


## Login com campos vazios:
**Cenário:** Usuário tenta logar sem preencher nenhum campo
**Pré-condição:** Nenhuma
**Passos:**
 Acessar a tela de login
 Deixar os campos de e-mail e senha em branco
 Clicar em "Entrar"

**Resultado esperado:** Sistema exibe mensagem de campo obrigatório e não permite o envio
**Status:**  Falhou 


##  Login com e-mail em formato inválido:
**Cenário:** Usuário insere um e-mail sem "@" ou domínio
**Pré-condição:** Nenhuma
**Passos:**
 Acessar a tela de login
 Inserir e-mail inválido: `usuarioteste.com`
 Inserir senha válida: `Senha123!`
 Clicar em "Entrar"

**Resultado esperado:** Sistema exibe mensagem "Formato de e-mail inválido"
**Status:** Passou


## CT005 — Bloqueio após múltiplas tentativas falhas:
**Cenário:** Usuário erra a senha 5 vezes seguidas
**Pré-condição:** Usuário previamente cadastrado no sistema
**Passos:**
 Acessar a tela de login
 Inserir e-mail válido e senha incorreta 5 vezes seguidas

**Resultado esperado:** Sistema bloqueia temporariamente novas tentativas e exibe aviso
**Status:**  Falhou 
