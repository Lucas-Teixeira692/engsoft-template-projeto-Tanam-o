# Documento de Requisitos

## Histórico de Revisões Deste Arquivo

| Data        | Versão | Descrição                     | Autor      |
|-------------|--------|-------------------------------|------------|
| 01/10/2023  | 1.0    | Versão inicial                 | Leonardo   |
| 05/10/2023  | 1.1    | Atualização dos requisitos     | Leonardo   |

---

## 1. Introdução

### 1.1 Propósito
O propósito deste documento é definir os requisitos funcionais e não funcionais para o sistema de fóruns acadêmicos moderados, que permitirá a interação entre alunos de diferentes instituições e cursos.

### 1.2 Escopo
O sistema abrangerá a criação e moderação de tópicos e postagens em fóruns organizados por curso e tema, com funcionalidades de autenticação, moderação e categorização.

### 1.3 Definições, Acrônimos e Abreviações
- **UFRJ**: Universidade Federal do Rio de Janeiro  
- **RF**: Requisitos Funcionais  
- **RNF**: Requisitos Não Funcionais  

---

## 2. Descrição Geral

### 2.1 Perspectiva do Produto
O produto será um sistema web que permitirá a interação entre alunos, facilitando a troca de informações e experiências acadêmicas. Ele se integrará a sistemas de autenticação existentes e poderá ser expandido para incluir notificações e perfis de usuários.

### 2.2 Funcionalidades do Produto
- Criação de tópicos em fóruns específicos.
- Resposta a tópicos existentes.
- Moderação de conteúdos.
- Sistema de denúncia para conteúdos impróprios.
- Autenticação de usuários.
- Exibição de informações sobre tópicos (data, autor, número de respostas).
- Categorização dos fóruns.

### 2.3 Características dos Usuários
- **Alunos**: Usuários que criarão e responderão a tópicos.
- **Moderadores**: Usuários responsáveis pela moderação dos conteúdos.
- **Administradores**: Usuários com acesso total ao sistema, incluindo gerenciamento de usuários e fóruns.

### 2.4 Restrições
- O sistema deve ser acessível apenas a usuários autenticados.
- Todos os conteúdos devem ser moderados antes da publicação.
- O sistema deve seguir as diretrizes de privacidade e segurança de dados.

---

## 3. Requisitos Específicos

### 3.1 Requisitos Funcionais

| ID    | Descrição                                                       | Prioridade |
|-------|-----------------------------------------------------------------|------------|
| RF01  | O usuário deve poder criar novos tópicos em fóruns específicos.  | Alta       |
| RF02  | O usuário deve poder responder a tópicos existentes.             | Alta       |
| RF03  | Todos os conteúdos devem ser moderados por administradores ou moderadores. | Alta       |
| RF04  | Deve haver um sistema de denúncia para conteúdos impróprios.     | Alta       |
| RF05  | O usuário deve estar autenticado para participar dos fóruns.     | Alta       |
| RF06  | Os tópicos devem mostrar data, autor e número de respostas.      | Média      |
| RF07  | Os fóruns devem estar categorizados por instituição, curso e área temática. | Média      |

### 3.2 Requisitos Não Funcionais

| ID    | Categoria    | Descrição                                         | Prioridade |
|-------|--------------|--------------------------------------------------|------------|
| RNF01 | Usabilidade  | O sistema deve ser intuitivo e fácil de usar.     | Alta       |
| RNF02 | Performance  | O sistema deve suportar até 1000 usuários simultâneos. | Alta       |
| RNF03 | Segurança    | O sistema deve garantir a segurança dos dados dos usuários. | Alta       |
| RNF04 | Manutenibilidade | O sistema deve ser fácil de manter e atualizar. | Média      |

---

## 4. Visão Geral do Sistema
O sistema será estruturado em uma arquitetura de backend que suportará a criação e moderação de posts e comentários, com um banco de dados relacional para armazenar informações sobre usuários, tópicos, postagens e denúncias.

---

## 5. Casos de Uso
Os casos de uso serão documentados em um documento separado, incluindo diagramas que ilustram as interações entre os usuários e o sistema.

---

## 6. Priorização de Requisitos
A priorização dos requisitos foi realizada com base na importância para a funcionalidade do sistema e na necessidade dos usuários, utilizando a técnica **MoSCoW** (_Must_, _Should_, _Could_, _Won't_).

---

## 7. Aprovação

| Nome       | Papel                   | Assinatura    | Data         |
|------------|-------------------------|---------------|--------------|
| Leonardo   | Analista de Requisitos   |               | 04/06/2025   |
| Lucas      | Gerente de Projeto       |               | 04/06/2025   |
