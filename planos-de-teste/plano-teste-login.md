# Plano de Teste — Tela de Login

## Objetivo:
Validar se a funcionalidade de login do sistema permite o acesso de usuários
com credenciais válidas e bloqueia o acesso de usuários com credenciais inválidas,
exibindo as mensagens de erro apropriadas.

## Escopo:
 Autenticação de usuário via e-mail e senha
 Mensagens de erro e validação de campos
 Comportamento do sistema após múltiplas tentativas falhas

## Fora do escopo:
 Recuperação de senha
 Autenticação via redes sociais (login social)

## Ambiente de teste:
 Navegador: Google Chrome (última versão estável)
 Sistema operacional: Windows 11
 Ambiente: Homologação

## Estratégia de teste:
 Testes funcionais manuais
 Testes de caso positivo (credenciais corretas)
 Testes de caso negativo (credenciais incorretas, campos vazios, formatos inválidos)

## Critérios de aceite:
 Usuário com credenciais válidas consegue acessar o sistema
 Usuário com credenciais inválidas recebe mensagem de erro clara
 Campos obrigatórios não podem ser enviados vazios
