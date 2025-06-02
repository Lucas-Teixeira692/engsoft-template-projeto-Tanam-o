# Caso de Teste: CT-001

## Título

Teste de Login com credenciais válidas

## Objetivo

Validar que o usuário consegue realizar login com um e-mail e senha válidos cadastrados no sistema.

## Requisitos/Histórias Relacionados

- Login e Cadastro
- SCRUM-4: Feedback (para avaliar se após login o sistema captura feedback corretamente)

## Pré-condições

1. O usuário deve estar previamente cadastrado no sistema.
2. O sistema deve estar online e disponível para autenticação.
3. O usuário deve possuir um e-mail e senha válidos.

## Dados de Teste

- E-mail: usuario@example.com
- Senha: Senha123

## Passos

1. Acessar a tela de login.
2. Inserir o e-mail “usuario@example.com” no campo correspondente.
3. Inserir a senha “Senha123” no campo correspondente.
4. Clicar no botão “Entrar” ou “Login”.

## Resultado Esperado

O sistema autentica o usuário e redireciona para a tela inicial (Home Screen), exibindo as funcionalidades disponíveis.

## Pós-condições

1. Usuário está logado e com sessão ativa.
2. Sistema mantém o estado do usuário para ações subsequentes.
3. Registro de login efetuado no sistema para fins de auditoria.

## Tipo de Teste

Sistema

## Automação

Manual

## Prioridade

Alta

## Observações

Verificar se o botão de "Esqueci minha senha" está visível para casos de erro na autenticação.
