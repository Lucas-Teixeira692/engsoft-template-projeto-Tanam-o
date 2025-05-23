## Documento de Arquitetura

### Histórico de Revisões

| Data       | Versão | Descrição             | Autor |
| :--------- | :----- | :-------------------- | :---- |
| 21/04/2025 | 1.0    | Versão inicial        | LT |
| 14/05/2025 | 1.1    | Detalhamento das metas, restrições, processos e melhorias com base nos documentos de teste e prototipagem. | LP |

### 1. Introdução

#### 1.1 Finalidade

O objetivo principal deste documento é descrever a arquitetura do sistema "Tá na Mão", uma plataforma projetada para facilitar o acesso e a retenção de informações acadêmicas essenciais para estudantes. Ele reúne recursos, orientações e oportunidades em uma plataforma segura e de fácil acesso.

#### 1.2 Escopo

O sistema "Tá na Mão" visa atender estudantes como seus principais usuários, juntamente com instituições afiliadas, como universidades. As funções do sistema incluem o acesso a informações sobre bolsas de estudo, apoio emocional, planos acessíveis, conteúdo universitário e assistência contínua. Módulos como websites, eLearning, CRMs, blogs, marketing e gestão de assinaturas do Odoo podem ser utilizados. O escopo da arquitetura abrange a definição do guia de estilo, a criação e evolução de protótipos, e a realização de testes de usabilidade.

#### 1.3 Definições, Acrônimos e Abreviações

* **Tá na Mão:** Nome do sistema/plataforma.
* **Odoo:** Software de gestão empresarial de código aberto.
* **CRM:** Customer Relationship Management.
* **UI:** User Interface (Interface do Usuário).
* **UX:** User Experience (Experiência do Usuário).
* **Placeholder:** Texto de exemplo dentro de um campo de entrada que descreve o formato ou tipo de entrada esperado.
* **SCRUM-1:** Informações sobre Bolsas.
* **SCRUM-2:** Suporte da Jinx.
* **SCRUM-3:** Notificações.
* **SCRUM-4:** Feedback.

### 2. Representação Arquitetural

#### 2.1 Modelo Arquitetural

O modelo arquitetural primário é baseado na **Criação de Protótipos Iterativos**, focado no design e refinamento da interface do usuário através de ciclos de feedback e ajuste. A arquitetura de interface segue um design consistente e minimalista, utilizando componentes padrão e um guia de estilo bem definido.

#### 2.2 Justificativa

A escolha de um modelo baseado em prototipagem iterativa é justificada pela necessidade de garantir usabilidade e estética desde as fases iniciais do projeto, permitindo ajustes rápidos com base em feedbacks internos e de usuários. A aplicação de um guia de estilo detalhado e o uso de componentes padrão reforçam a consistência do design, facilitando a manutenção e a usabilidade (segundo Nielsen, 1994). Isso está alinhado com as boas práticas de design.

### 3. Metas e Restrições da Arquitetura

#### 3.1 Metas

* Facilitar o acesso e a retenção de informações acadêmicas essenciais para estudantes.
* Fornecer uma plataforma segura e de fácil acesso.
* Oferecer funcionalidades como acesso a bolsas de estudo, apoio emocional, planos acessíveis, conteúdo universitário e assistência contínua.
* Garantir uma interface de usuário clara, coerente e com boa usabilidade.
* Transmitir uma sensação de profissionalismo e convite à ação através da combinação de cores.
* Garantir a uniformidade no uso de fontes e tamanhos para acessibilidade.
* Garantir que a documentação final seja impecável, detalhando problemas, priorização e melhorias.
* Assegurar que a descrição das tarefas e papéis nos testes esteja clara.
* Manter a estrutura da documentação clara e acessível, compilando o feedback de forma organizada.

#### 3.2 Restrições

* A seleção de logotipo e ícones deve seguir um estilo monocromático e minimalista.
* O alinhamento do cabeçalho nas telas deve ser central ou no canto superior esquerdo.
* Os ícones devem ter um estilo outline simples, mantendo um tamanho de 24px a 32px.
* A cor dos placeholders foi ajustada para `#CCCCCC` para melhorar a leitura.
* A arquitetura deve considerar a integração com módulos Odoo para funcionalidades como websites, eLearning, CRMs, blogs, marketing e gestão de assinaturas.

### 4. Visão de Casos de Uso

#### 4.1 Diagrama de Casos de Uso

Não foram fornecidos diagramas de casos de uso específicos, mas os protótipos de login e cadastro (Imagens 1 e 2 no arquivo "Tá na Mão (2) HD.pdf") indicam os principais fluxos iniciais de interação do usuário.

#### 4.2 Descrição dos Casos de Uso Significativos

* **Login de Usuário:** Permite que o usuário acesse o sistema inserindo seu email/usuário e senha.
* **Cadastro de Usuário:** Permite que novos usuários criem uma conta fornecendo seu nome de usuário, e-mail e senha.
* **Acessar Bolsas de Estudo:** O usuário pode acessar informações sobre bolsas de estudo.
* **Obter Apoio Emocional:** O usuário pode acessar recursos de apoio emocional.
* **Acessar Conteúdo Universitário:** O usuário pode acessar conteúdo relevante à universidade.
* **Receber Notificações:** O sistema envia notificações (push, e-mail, etc.) sobre informações importantes.
* **Fornecer Feedback:** O usuário pode enviar feedback sobre a plataforma através de um sistema dedicado (pesquisas, entrevistas, formulários).
* **Acessar Suporte (Jinx):** O usuário pode acessar materiais de suporte (tutoriais, FAQs) e resolver tickets de suporte.

### 5. Visão Lógica

#### 5.1 Visão Geral

A organização lógica do sistema é centrada na interface do usuário e na experiência de interação. Ela é definida por um guia de estilo que dita a paleta de cores, tipografia e componentes padrão, garantindo consistência visual e funcional. Elementos de interface como botões e campos de entrada são refinados para usabilidade e estética.

#### 5.2 Pacotes de Design Significativos

* **Paleta de Cores:** Define as cores primárias e secundárias do sistema, incluindo Azul Escuro (`#0049A8`), Azul Claro (`#3B6AD1`), Roxo Claro (`#A793E7`), Roxo Pastel (`#AEA3CE`), Branco (`#FFFFFF`) e Preto Translúcido (`#00000080`).
* **Tipografia:** Define a fonte principal como Poppins, sans-serif, com tamanhos padrão para título (24px, bold), texto comum (14px) e texto auxiliar (12px).
* **Componentes Padrão:** Inclui botões (Primário: fundo `#A793E7`, texto `#000000` bold, borda arredondada 8px, hover `#8C76D1`; Secundário/Links: cor `#FFFFFF`, texto sublinhado ou bold para destaque, sem borda), e campos de entrada (borda none, fundo `#AEA3CE` translúcido, placeholder cinza claro `#CCCCCC`, borda arredondada 8px).
* **Ícones e Elementos Gráficos:** Logo (Capelo acadêmico preto com estrelas e o texto "Tá na Mão"), estilo dos ícones (Flat, monocromáticos ou outline simples), e tamanho sugerido de 24px a 32px.
* **Layouts:** Define os padrões de alinhamento para cabeçalhos (central ou superior esquerdo).
* **Linguagem para Mensagens ao Usuário:** Inclui mensagens padronizadas para sucesso, erro, cadastro e ajuda.

#### 5.3 Diagramas de Classes

Não foram fornecidos diagramas de classes explícitos.

### 6. Visão de Processos

O processo principal é o ciclo iterativo de prototipagem e avaliação. Isso inclui: planejamento do guia de estilo, criação de protótipos iniciais, evolução dos protótipos com base em feedback, e testes de usabilidade. As atividades do projeto são organizadas em Sprints SCRUM, conforme detalhado no documento "Condução de Testes do Tá na Mão.pdf":

* **SCRUM-1: Informações sobre Bolsas:**
    * **Reunião de Planejamento do Sprint:** Definir quais informações sobre bolsas devem ser incluídas.
    * **Desenvolvimento:** Coletar dados relevantes sobre bolsas; Criar conteúdo informativo (textos, gráficos).
    * **Revisão:** Revisar e ajustar as informações coletadas com o time.
    * **Demonstração:** Apresentar as informações sobre bolsas para as partes interessadas.
* **SCRUM-2: Suporte da Jinx:**
    * **Reunião de Planejamento do Sprint:** Identificar as principais necessidades de suporte para a ferramenta.
    * **Desenvolvimento:** Criar material de suporte (tutoriais, FAQs); Resolver tickets de suporte abertos pelos usuários.
    * **Revisão:** Analisar a eficácia do suporte oferecido e fazer melhorias.
    * **Demonstração:** Mostrar as melhorias e novos materiais criados para o suporte.
* **SCRUM-3: Notificações:**
    * **Reunião de Planejamento do Sprint:** Listar os tipos de notificações necessárias e sua urgência.
    * **Desenvolvimento:** Implementar a funcionalidade de notificações (push, e-mail, etc.); Testar o envio e a entrega das notificações.
    * **Revisão:** Revisar o funcionamento das notificações com o time.
    * **Demonstração:** Apresentar a funcionalidade de notificações em funcionamento.
* **SCRUM-4: Feedback:**
    * **Reunião de Planejamento do Sprint:** Decidir sobre os métodos de coleta de feedback (pesquisas, entrevistas, formulários).
    * **Desenvolvimento:** Criar e implementar um sistema para coletar feedback; Elaborar formulários de feedback eficazes.
    * **Revisão:** Analisar o feedback coletado e priorizar melhorias.
    * **Demonstração:** Compartilhar os resultados do feedback e as ações planejadas.

### 7. Visão de Implantação

#### 7.1 Diagrama de Implantação

Não foram fornecidos diagramas de implantação explícitos.

#### 7.2 Descrição dos Nós

Não foram fornecidas informações específicas sobre nós de implantação.

### 8. Visão de Implementação

#### 8.1 Visão Geral

A implementação é guiada pelo guia de estilo e pelos protótipos desenvolvidos, utilizando ferramentas de prototipagem (Figma/Adobe XD). A interface é construída com foco na aplicação do esquema de cores e fontes definidos. O processo de refinamento dos protótipos inclui a análise de feedback e a implementação de melhorias, como o ajuste da cor dos placeholders para `#CCCCCC` para melhor legibilidade.

#### 8.2 Camadas

Embora não explicitamente definidas, as atividades sugerem uma separação lógica entre:

* **Camada de Apresentação/UI:** Responsável pela renderização das telas de login, cadastro e mensagens ao usuário, e pela interação com o usuário.
* **Camada de Negócios:** (Implícita) Gerencia as funcionalidades relacionadas a bolsas de estudo, apoio emocional, planos acessíveis, conteúdo universitário, notificações, e sistema de feedback.
* **Camada de Dados:** (Implícita) Lida com o acesso e persistência das informações de usuário (email/usuário, nome, senha) e dados relacionados às funcionalidades do sistema.

### 9. Visão de Dados

#### 9.1 Modelo de Dados

Não foi fornecido um modelo de dados explícito, mas o sistema manipula dados de usuário (email/usuário, nome, senha) e informações acadêmicas (bolsas de estudo, conteúdo universitário), além de dados de feedback e suporte.

### 10. Tamanho e Performance

Não foram fornecidos objetivos ou restrições específicas de tamanho e performance. No entanto, a busca por clareza e facilidade de navegação nos testes de usabilidade sugere um foco na otimização da experiência do usuário, o que indiretamente contribui para a percepção de performance.

### 11. Qualidade

A qualidade é abordada principalmente através de:

* **Usabilidade:** Realização de testes com usuários internos para avaliar clareza e facilidade de navegação. Ajustes foram feitos, como a cor dos placeholders, para melhorar a leitura. O Roteiro de Teste de Usabilidade foi considerado bem estruturado e as Histórias de Usuário claras.
* **Estética:** A aplicação do guia de estilo e o refinamento de elementos de interface visam garantir a beleza do design. A combinação de cores transmite profissionalismo e convite à ação.
* **Consistência:** O uso de componentes padrão segue as boas práticas de design consistente, facilitando a manutenção e usabilidade (segundo Nielsen, 1994). A uniformidade no uso das fontes e tamanhos garante um design consistente.
* **Acessibilidade:** A uniformidade no uso de fontes e tamanhos é reforçada para garantir a acessibilidade.
* **Clareza da Documentação:** Há um foco contínuo em garantir que a documentação final seja impecável, com detalhamento conciso dos problemas identificados, sua priorização e as melhorias implementadas. A descrição das tarefas e os papéis nos testes devem ser claros, e o feedback compilado de forma organizada para fácil identificação de aspectos positivos e sugestões.

### 12. Princípios SOLID Aplicados

Não há menção explícita à aplicação dos princípios SOLID nas informações fornecidas.

### 13. Padrões de Design Utilizados

* **Guia de Estilo / Design System:** A definição de paleta de cores, tipografia e componentes padrão age como um sistema de design, garantindo consistência.
* **Prototipagem Iterativa:** O ciclo de criação, ajuste e teste de protótipos é um padrão de desenvolvimento focado na melhoria contínua.
* **Visual Hierarchy (Teoria do Olhar):** Aplicada ao posicionamento do cabeçalho e mensagens ao usuário para melhor navegação.
* **Scrum:** As atividades de desenvolvimento são organizadas em Sprints com responsabilidades definidas para cada SCRUM (Informações sobre Bolsas, Suporte da Jinx, Notificações, Feedback), incluindo reuniões de planejamento, desenvolvimento, revisão e demonstração.
>[!TIP]
>Ao longo do desenvolvimento, revise este documento para garantir que a implementação esteja alinhada com a arquitetura planejada. Documente as decisões arquiteturais importantes, incluindo as alternativas consideradas e os motivos da escolha final.
