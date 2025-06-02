# Caso de Uso: 001

## Nome

Cadastro e Login com Validação Institucional

## Descrição

Este caso de uso descreve o processo de cadastro e login de usuários utilizando e-mails institucionais da UFPE, garantindo que apenas membros da comunidade acadêmica tenham acesso à plataforma.

## Atores

- Ana Ribeiro (Usuária Primária)
- Sistema de E-mail (Ator Secundário)

## Pré-condições

1. O usuário deve ter um e-mail institucional válido terminando em `@ufpe.br`.
2. O sistema de envio de e-mails deve estar ativo.
3. O usuário não deve ter um cadastro anterior com o mesmo e-mail.

## Fluxo Básico

1. Ana Ribeiro acessa a página de cadastro.
2. Ela insere seu e-mail institucional e cria uma senha.
3. O sistema valida o e-mail e envia um e-mail de verificação.
4. Ana verifica seu e-mail e clica no link de ativação.
5. O sistema ativa a conta e permite o login.
6. Ana faz login com seu e-mail e senha.

## Fluxos Alternativos

### Alternativa 1: E-mail não institucional

1. Ana tenta se cadastrar com um e-mail que não termina em `@ufpe.br`.
2. O sistema exibe uma mensagem de erro amigável.
3. Ana corrige o e-mail e tenta novamente.

### Alternativa 2: E-mail já cadastrado

1. Ana tenta se cadastrar com um e-mail já existente no sistema.
2. O sistema exibe uma mensagem informando que o e-mail já está em uso.
3. Ana pode optar por recuperar a senha ou usar um e-mail diferente.

## Fluxos de Exceção

### Exceção 1: Falha no envio de e-mail

1. O sistema falha ao enviar o e-mail de verificação.
2. O sistema exibe uma mensagem de erro informando a falha.
3. Ana pode tentar novamente ou entrar em contato com o suporte.

### Exceção 2: Link de ativação expirado

1. Ana tenta ativar a conta com um link de ativação expirado.
2. O sistema exibe uma mensagem informando que o link não é mais válido.
3. Ana deve solicitar um novo e-mail de verificação.

## Pós-condições

1. O usuário está cadastrado e pode acessar a plataforma.
2. O sistema registra a atividade de cadastro e login.
3. O e-mail de verificação é enviado e gerenciado pelo sistema.

## Requisitos Relacionados

- O sistema deve validar o formato do e-mail.
- O sistema deve garantir a segurança da autenticação.
- O sistema deve permitir a recuperação de senha.

## Interface de Usuário

- A página de cadastro deve incluir campos para e-mail e senha, além de mensagens de erro.
- A página de login deve ter campos para e-mail e senha, com opção de recuperação de senha.

## Diagrama

```mermaid
flowchart TD
        A(["Início"])
        A --> B{"Decisão"}
        B --> C["Cadastro com e-mail válido"]
        B --> D["Cadastro com e-mail inválido"]
        C --> E["E-mail de verificação enviado"]
        D --> F["Mensagem de erro exibida"]
        E --> G["Ativação da conta"]
        G --> H["Login permitido"]
