# História de Usuário: Lucas Martins

## Título
Criação e resposta em fóruns acadêmicos moderados

## Narrativa
**Como** Lucas Martins, aluno de Administração na UFRJ,  
**Eu quero** criar tópicos e responder dúvidas em fóruns organizados por curso e tema,  
**Para que** trocar experiências acadêmicas com colegas de outras regiões e obter ajuda rápida para questões relacionadas a disciplinas e estágios.

## Critérios de Aceitação
- [ ] O usuário deve poder criar novos tópicos em fóruns específicos por curso e tema.
- [ ] O usuário deve poder responder a tópicos existentes com comentários.
- [ ] Todos os conteúdos devem ser moderados por administradores ou moderadores nomeados.
- [ ] Deve haver um sistema de denúncia para conteúdos impróprios.
- [ ] O usuário deve estar autenticado para participar dos fóruns.
- [ ] Os tópicos devem mostrar data, autor e número de respostas.
- [ ] Os fóruns devem estar categorizados por instituição, curso e área temática (ex: Estágio, TCC, Dúvidas de disciplina).

## Detalhes Técnicos
- Backend com suporte a criação e moderação de posts e comentários.
- Organização em estrutura hierárquica: Instituição > Curso > Tópico > Postagens.
- Banco de dados relacional com tabelas para usuários, tópicos, postagens e denúncias.
- Painel administrativo para moderadores (ex: aprovação, exclusão, bloqueio).
- Possibilidade futura de upvotes/downvotes ou destaque de respostas úteis.

## Dependências
- Sistema de autenticação implementado.
- Cadastro de cursos e temas acadêmicos na base da plataforma.
- Política de moderação definida.

## Estimativa
**8 Story Points**

## Prioridade
**Must**

## Observações
- Importante manter ambiente saudável e construtivo.
- Pode ser útil integrar sistema de notificações (ex: alertar quando houver resposta a um tópico seguido).
- Considerar integração com perfil do usuário (ex: exibir contribuições nos fóruns).
