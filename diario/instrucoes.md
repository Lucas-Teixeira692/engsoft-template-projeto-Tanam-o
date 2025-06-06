```
# Plataforma Educacional "Tá na Mão"

---

## Introdução

Esta proposta integra a tese de desenvolvimento de uma plataforma educacional online voltada para estudantes universitários com um plano de testes detalhado já elaborado para o sistema "Tá na Mão". A iniciativa visa centralizar informações institucionais, fortalecer a comunicação entre alunos e promover o acesso facilitado a conteúdos acadêmicos, criando um ambiente digital dinâmico, seguro e adaptável às demandas educacionais contemporâneas.

---

## 1. Objetivos do Projeto

- Centralizar informações acadêmicas e institucionais adaptadas conforme a universidade e região do usuário.
- Fortalecer a comunicação entre alunos por meio de funcionalidades colaborativas e personalizadas.
- Facilitar o acesso a conteúdos e processos administrativos essenciais (vestibulares, matrículas, prazos).
- Construir uma comunidade acadêmica ativa e focada em temas educacionais.
- Possibilitar expansão futura com materiais de estudo e monetização sustentável.

---

## 2. Estrutura da Plataforma

A proposta do sistema está organizada em cinco eixos principais:

| Eixo | Descrição |
|-------|-----------|
| 1. Feed de Notícias | Página estilo rede social com notícias e conteúdos acadêmicos atualizados e personalizados. |
| 2. Documentação Personalizada | Apresentação de requisitos e prazos acadêmicos conforme o perfil regional e institucional do usuário. |
| 3. Sistema de Favoritos | Permite salvar cursos, bolsas e instituições de interesse para acesso rápido. |
| 4. Comunidade / Fóruns | Espaço inspirado no modelo Reddit com fóruns exclusivos, moderação eficaz e foco acadêmico. |
| 5. Expansão & Monetização | Preparação para adicionar materiais de estudo e recursos pagos no futuro. |

---

## 3. Plano de Testes Integrado

### 3.1 Objetivos do Plano de Testes

- Assegurar qualidade, funcionalidade e usabilidade conforme os objetivos da plataforma.
- Identificar e corrigir falhas antes do lançamento oficial.
- Validar a consistência da interface e a eficácia da comunicação entre usuários.
- Avaliar a experiência do usuário final incluindo feedback e facilidade de uso.

### 3.2 Escopo dos Testes

- Funcionalidades principais (SCRUM-1 a SCRUM-4) e sistemas de Login/Cadastro.
- Interfaces e elementos de navegação, incluindo correções textuais e reorganização dos conteúdos.
- Aspectos não funcionais como segurança, performance e consistência visual.

### 3.3 Metodologia e Níveis de Teste

- **Testes Unitários** para componentes individuais, realizados por desenvolvedores.
- **Testes de Integração** para interações entre módulos.
- **Testes de Sistema** para validação ponta a ponta da plataforma.
- **Testes de Usabilidade** focados na experiência e coleta de feedback dos usuários.
- **Testes de Regressão** para garantir a estabilidade após atualizações ou correções.

### 3.4 Critérios de Entrada e Saída

| Tipo de Teste   | Entrada                               | Critério de Saída                                 |
|-----------------|-------------------------------------|--------------------------------------------------|
| Unitário        | Código desenvolvido e revisado      | Componentes funcionais e sem erros                |
| Integração      | Módulos testados unitariamente      | Módulos interagindo corretamente                  |
| Sistema         | Plataforma integrada                 | Funcionalidades conformes aos requisitos          |
| Usabilidade     | Protótipos ou versão funcional      | Feedback detalhado com identificação de melhorias |
| Regressão       | Nova versão com alterações           | Funcionalidades anteriores preservadas             |

### 3.5 Ferramentas de Teste

- GitHub para controle de versão.
- Jira para gestão de tarefas e bugs.
- Visual Studio Code para desenvolvimento.
- Figma para prototipagem e design.
- Postman para testes de APIs.

---

## 4. Organização e Responsabilidades

| SCRUM       | Responsáveis                        | Principais Atividades                                  |
|-------------|-----------------------------------|------------------------------------------------------|
| SCRUM-1     | Leonardo, João Pedro, Lucas (rev) | Conteúdos sobre bolsas, revisão e apresentação        |
| SCRUM-2     | Leonardo, João Pedro, Lucas (rev) | Desenvolvimento e suporte Jinx, resolução de tickets  |
| SCRUM-3     | Sophia, Lucas (rev)                | Implementação e teste de notificações                  |
| SCRUM-4     | João Pedro, Lucas (rev)            | Coleta e análise de feedback, elaboração de relatórios |

---

## 5. Prioridades no Desenvolvimento e Testes

- **Prioridade Alta:**
  - Clareza e qualidade das documentações.
  - Funcionamento básico e correto de login e cadastro.
  - Correções textuais, de rotulagem e navegação.

- **Prioridade Média:**
  - Aperfeiçoamento dos sistemas de feedback e notificações.
  - Refinamento das funcionalidades baseadas no retorno dos testes.

- **Prioridade Baixa:**
  - Aprimoramento geral da documentação para o relatório final.

---

## 6. Considerações Finais da Tese Integrada

A plataforma “Tá na Mão” propõe um ambiente digital inovador para estudantes universitários, visando superar lacunas informacionais e promover colaboração acadêmica. O desenvolvimento estratégico, aliado a um rigoroso plano de testes e clareza nas responsabilidades, deve assegurar um produto robusto, intuitivo e alinhado às demandas reais dos usuários. A continuidade dos esforços em moderação e monetização garantirá sua sustentabilidade futura.

---

## 7. Design e Experiência do Usuário (GUI)

Inspirados pelas melhores práticas de design minimalista e elegante, a plataforma adotará:

### Visual

- Fundo claro (#ffffff) com ampla área para respirar.
- Tipografia sofisticada e hierárquica para títulos (48px+, peso 600-800).
- Texto do corpo em cinza neutro (#6b7280), legível e confortável (16-18px).
- Cartões e seções com cantos arredondados subtis (~0.75rem) e sombras leves.
- Ícones simples e monocromáticos.

### Layout

- Layout responsivo full-width com container centralizado (max-width 1200px).
- Separação visual clara por meio de espaços generosos, sem linhas explícitas.
- Uso coordenado de grid e colunas flexíveis para blocos de conteúdo.
- Seções empilhadas verticalmente com espaçamento consistente (ex: pt-16 pb-20).

### Navegação & Header

- Navegação top sticky minimalista com logo à esquerda e ítens à direita.
- CTA destacado no hero (“Explore a Plataforma”), com botões amplos, com boa separação visual e hover suave.

### Interatividade

- Transições suaves em botões e cartões (hover/active).
- Formulários simplificados com campos claramente rotulados e espaçamento adequado.
- Alternância visual de temas considerada para futuro desenvolvimento.

---

## 8. Próximos Passos

- Desenvolvimento do mapa mental para visualização da arquitetura da plataforma.
- Efetivação das estratégias de moderação para manter ambiente seguro e acadêmico.
- Planejamento detalhado para as fases iniciais de monetização.
- Continuidade dos testes integrados baseados no plano e feedbacks do público-alvo.

---

Este documento serve como um guia articulado para o desenvolvimento integrado, testes e experiência do usuário da plataforma educacional “Tá na Mão”, garantindo alinhamento da visão técnica, operacional e de usabilidade.
```
