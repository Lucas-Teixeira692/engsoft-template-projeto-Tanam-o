# História de Usuário: Ana Ribeiro

## Título

Cadastro e login com validação institucional

## Narrativa

**Como** Ana Ribeiro, estudante de Engenharia Civil na UFPE,  
**Eu quero** me cadastrar e fazer login usando meu e-mail institucional (@ufpe.br),  
**Para que** acessar conteúdos exclusivos da plataforma, participar dos fóruns da minha universidade e garantir que apenas membros reais da comunidade acadêmica estejam presentes.

## Critérios de Aceitação

- [ ] O sistema deve permitir cadastro apenas com e-mails terminados em `@ufpe.br`.
- [ ] Um e-mail de verificação deve ser enviado após o cadastro, contendo um link para ativação da conta.
- [ ] O login só será permitido após a verificação do e-mail institucional.
- [ ] Caso o usuário tente cadastrar um e-mail que não seja `@ufpe.br`, uma mensagem de erro amigável deve ser exibida.
- [ ] O sistema deve validar o formato do e-mail e garantir que não haja duplicidade de cadastro.
- [ ] A autenticação deve ser segura e seguir boas práticas (ex: senha criptografada, uso de HTTPS, etc).

## Detalhes Técnicos

- Validação do domínio do e-mail (`@ufpe.br`) no backend.
- Envio de e-mail de verificação (ex: via SendGrid ou Amazon SES).
- Armazenamento seguro de senhas (ex: hash com bcrypt).
- Autenticação via tokens JWT ou sessões.
- Backend com suporte a verificação por link único/token temporário.

## Dependências

- Sistema de envio de e-mails ativo.
- Infraestrutura de autenticação disponível.
- Frontend com páginas de cadastro, login e confirmação de e-mail.

## Estimativa

**5 Story Points**

## Prioridade

**Must**

## Observações

- Considerar suporte futuro a SSO institucional (ex: login com Sigepe ou Google Acadêmico da UFPE).
- Incluir testes automatizados para o fluxo completo de autenticação.
- Pode haver exceções para e-mails institucionais de professores com subdomínios.
