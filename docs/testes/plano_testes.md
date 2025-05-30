# Histórico de Revisões

| Data       | Versão | Descrição                | Autor  |
| ---------- | ------ | ------------------------ | ------ |
| 17/09/2024 | 1.0    | Ideia inicial           | [Sophia] |
| 25/04/2025 | 1.5    | Versão Alfa        | [Lucas T] |
| 25/04/2025 | 2.0    | Versão Beta        | [Lucas T e Leo P] |



# 1. Introdução

Este documento descreve o plano de testes para o sistema "Tá na Mão", uma plataforma projetada para facilitar o acesso a informações acadêmicas essenciais para estudantes e instituições de ensino. O objetivo principal é garantir a qualidade, funcionalidade e usabilidade do sistema, assegurando que ele atenda aos requisitos definidos e ofereça uma experiência satisfatória aos usuários.

## 1.1 Objetivos

* Garantir que todas as funcionalidades estejam operacionais e de acordo com os requisitos.
* Identificar e corrigir defeitos e falhas no sistema.
* Validar a usabilidade e a experiência do usuário.
* Assegurar a consistência e clareza da linguagem e das interfaces.
* Verificar a eficácia do sistema de feedback para capturar informações relevantes.

## 1.2 Escopo

O escopo dos testes abrange as principais funcionalidades do sistema "Tá na Mão", incluindo:
* Informações sobre Bolsas (SCRUM-1)
* Suporte da Jinx (SCRUM-2)
* Notificações (SCRUM-3)
* Feedback (SCRUM-4)
* Funcionalidades de Login e Cadastro
* Interfaces do usuário, com foco em correção textual, rotulagem, reorganização de espaço e conteúdo, e ajustes nos elementos de navegação

# 2. Estratégia de Teste

O grupo auxilia em praticamente todas as partes e depois, apenas dois testam as funcionalidades

## 2.1 Níveis de Teste

* **Testes Unitários**: Serão realizados pelos desenvolvedores para testar componentes individuais do código.
* **Testes de Integração**: Testarão a interação entre diferentes módulos e funcionalidades do sistema.
* **Testes de Sistema**: Validarão o sistema como um todo, garantindo que todas as funcionalidades atendam aos requisitos.
* **Testes de Usabilidade**: Avaliarão a facilidade de uso e a experiência do usuário, baseando-se no feedback dos usuários.
* **Testes de Regressão**: Serão executados para garantir que as novas alterações não introduzam novos defeitos ou causem impacto negativo em funcionalidades existentes.

## 2.2 Ferramentas

* GitHub; Jira; Visual Studio Code.
* Figma; Mermaid.
* Postman
  
# 3. Recursos

## 3.1 Ambientes de Teste

* Visual Studio Code.
* Figma; Jira.

## 3.2 Equipe

* **Lucas Teixeira (Líder do Grupo/Revisão e Organização)**
* **Leonardo Silveira Pontolio (Escrita dos Documentos)**
* **Sophia Victoria Santos (Organização de Documentações e Tópicos)**
* **João Pedro Meira da Silva Braz de Mattos (Escrita dos Documentos)**
* **João Vitor Teles (Revisão dos Documentos)**

# 4. Critérios

## 4.1 Critérios de Entrada

* **Testes Unitários**: Código desenvolvido e revisado
* **Testes de Integração**: Módulos unitariamente testados
* **Testes de Sistema**: Sistema integrado e pronto para testes de ponta a ponta
* **Testes de Usabilidade**: Protótipos ou versão funcional do sistema
* **Testes de Regressão**: Nova versão do sistema com alterações ou correções

## 4.2 Critérios de Saída

* **Testes Unitários**: Componentes individuais funcionando conforme o esperado, sem erros
* **Testes de Integração**: Interação correta entre os módulos
* **Testes de Sistema**: Sistema funcionando conforme os requisitos funcionais e não funcionais
* **Testes de Usabilidade**: Coleta de feedback detalhado sobre a usabilidade e identificação de pontos de melhoria
* **Testes de Regressão**: Confirmação de que as funcionalidades existentes não foram impactadas negativamente

# 5. Itens de Teste

## 5.1 Funcionalidades a serem testadas

* SCRUM-1: Informações sobre Bolsas
	+ Coleta, criação e revisão de conteúdo informativo sobre bolsas
	+ Verificação da precisão e completude das informações
* SCRUM-2: Suporte da Jinx
	+ Criação de material de suporte (tutoriais, FAQs) e resolução de tickets
	+ Verificação da eficácia do suporte
* SCRUM-3: Notificações
	+ Implementação e teste da funcionalidade de notificações (push, e-mail)
	+ Verificação da entrega e conteúdo das notificações
* SCRUM-4: Feedback
	+ Criação de sistema para coletar feedback dos usuários e elaboração de formulários
	+ Verificação da coleta e análise do feedback
* Login
	+ Preenchimento de e-mail/usuário e senha, botão de acesso, e opção de cadastro
	+ Verificação da autenticação e autorização
* Cadastro
	+ Preenchimento de usuário, e-mail e senha, botão de cadastrar, e link para login
	+ Verificação da criação de conta e login

## 5.2 Características não-funcionais a serem testadas

* Usabilidade
	+ Facilidade de uso da interface
	+ Clareza das mensagens
* Consistência
	+ Aplicação do guia de estilo (cores, tipografia, componentes) em todas as telas
* Performance
	+ Tempo de resposta do sistema
* Segurança
	+ Proteção dos dados do usuário

## 5.3 Interfaces a serem testadas

* Interface de Login
	+ Campos de entrada, botão de acesso, link para cadastro
* Interface de Cadastro
	+ Campos de entrada, botão de cadastrar, link para login
* Home Screen
	+ Estrutura com menu lateral e áreas para conteúdo
* Elementos de Navegação
	+ Botão "Voltar" e renomeação de botões

# 6. Priorização dos itens

1.  **Prioridade Alta**:
	* Detalhar problemas e melhorias na documentação final
	* Clareza na descrição das tarefas e papéis nos testes
	* Compilação organizada do feedback
	* Correções textuais e de rotulagem, e ajustes nos elementos de navegação
	* Funcionamento básico de Login e Cadastro
2.  **Prioridade Média**:
	* Detalhar dificuldades do usuário no relatório de feedback do SCRUM-4
	* Revisão do sistema de feedback para coletar informações relevantes
	* Refinamento dos protótipos de Informações sobre Bolsas (SCRUM-1), Suporte da Jinx (SCRUM-2), e Notificações (SCRUM-3) com base no feedback
3.  **Prioridade Baixa**:
	* Aprimoramentos na documentação final das histórias de usuário e organização geral

# 7. Critérios de Sucesso

## 7.1 Métricas para avaliar a eficácia dos testes

* Porcentagem de casos de teste executados com sucesso = 75%
* Feedback positivo dos usuários em relação à usabilidade = 50%
* Aderência às diretrizes do guia de estilo

## 7.2 Critérios de cobertura mínima

* Cobertura de 100% dos requisitos funcionais
* Cobertura de 80% dos requisitos não funcionais

## 7.3 Nível aceitável de defeitos

* Zero defeitos críticos ou de alta prioridade no lançamento
* Número mínimo de defeitos de média e baixa prioridade, com plano de correção para futuras iterações

