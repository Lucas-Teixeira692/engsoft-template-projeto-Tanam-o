# Matriz de Rastreabilidade de Requisitos

## Histórico de Revisões deste Arquivo

| Data       | Versão | Descrição                                     | Autor      |
| ---------- | ------ | --------------------------------------------- | ---------- |
| 02-04-2025 | 1.0    | Matriz inicial baseada nos documentos fornecidos | Lucas T |
| 15-05-2025 | 1.1    | Atualização com requisitos da tese e ajustes finais | Lucas T |

---

## 1. Introdução

Este documento apresenta a matriz de rastreabilidade dos requisitos da plataforma educacional online "Tá na Mão", permitindo visualizar as relações entre requisitos, casos de uso, componentes do sistema e casos de teste para garantir a integridade e a cobertura dos requisitos durante o desenvolvimento.

---

## 2. Matriz de Rastreabilidade

### 2.1 Requisitos x Casos de Uso

| Requisito                                    | UC01 (Login) | UC02 (Cadastro) | UC03 (Feed de Notícias) | UC04 (Documentação Personalizada) | UC05 (Sistema de Favoritos) | UC06 (Comunidade/Fóruns) | UC07 (Notificações) | UC08 (Feedback) | UC09 (Suporte) |
| :------------------------------------------- | :----------- | :-------------- | :---------------------- | :-------------------------------- | :-------------------------- | :----------------------- | :------------------ | :-------------- | :------------- |
| RF01 - Login de Usuário                       | X            |                 |                         |                                   |                             |                          |                     |                 |                |
| RF02 - Cadastro de Usuário                    |              | X               |                         |                                   |                             |                          |                     |                 |                |
| RF03 - Acesso ao Feed de Notícias             |              |                 | X                       |                                   |                             |                          |                     |                 |                |
| RF04 - Sistema de Documentação Personalizada |              |                 |                         | X                                 |                             |                          |                     |                 |                |
| RF05 - Sistema de Favoritos                    |              |                 |                         |                                   | X                           |                          |                     |                 |                |
| RF06 - Comunidade e Fóruns                     |              |                 |                         |                                   |                             | X                        |                     |                 |                |
| RF07 - Envio de Notificações                   |              |                 |                         |                                   |                             |                          | X                   |                 |                |
| RF08 - Coleta e Análise de Feedback            |              |                 |                         |                                   |                             |                          |                     | X               |                |
| RF09 - Suporte via tutoriais e tickets         |              |                 |                         |                                   |                             |                          |                     |                 | X              |

### 2.2 Requisitos x Componentes do Sistema

| Requisito                                    | Módulo Login | Módulo Cadastro | Módulo Feed | Módulo Documentação | Módulo Favoritos | Módulo Comunidade | Módulo Notificações | Módulo Feedback | Módulo Suporte |
| :------------------------------------------- | :----------- | :-------------- | :---------- | :------------------ | :--------------- | :---------------- | :------------------ | :-------------- | :------------- |
| RF01 - Login de Usuário                       | X            |                 |             |                     |                  |                   |                     |                 |                |
| RF02 - Cadastro de Usuário                    |              | X               |             |                     |                  |                   |                     |                 |                |
| RF03 - Acesso ao Feed de Notícias             |              |                 | X           |                     |                  |                   |                     |                 |                |
| RF04 - Sistema de Documentação Personalizada |              |                 |             | X                   |                  |                   |                     |                 |                |
| RF05 - Sistema de Favoritos                    |              |                 |             |                     | X                |                   |                     |                 |                |
| RF06 - Comunidade e Fóruns                     |              |                 |             |                     |                  | X                 |                     |                 |                |
| RF07 - Envio de Notificações                   |              |                 |             |                     |                  |                   | X                   |                 |                |
| RF08 - Coleta e Análise de Feedback            |              |                 |             |                     |                  |                   |                     | X               |                |
| RF09 - Suporte via tutoriais e tickets         |              |                 |             |                     |                  |                   |                     |                 | X              |

### 2.3 Requisitos x Casos de Teste

| Requisito                                    | CT01 (Testes Login) | CT02 (Testes Cadastro) | CT03 (Testes Feed) | CT04 (Testes Documentação) | CT05 (Testes Favoritos) | CT06 (Testes Comunidade) | CT07 (Testes Notificações) | CT08 (Testes Feedback) | CT09 (Testes Suporte) |
| :------------------------------------------- | :------------------ | :--------------------- | :----------------- | :------------------------- | :---------------------- | :---------------------- | :------------------------- | :-------------------- | :-------------------- |
| RF01 - Login de Usuário                       | X                   |                        |                    |                            |                         |                         |                            |                       |                       |
| RF02 - Cadastro de Usuário                    |                     | X                      |                    |                            |                         |                         |                            |                       |                       |
| RF03 - Acesso ao Feed de Notícias             |                     |                        | X                  |                            |                         |                         |                            |                       |                       |
| RF04 - Sistema de Documentação Personalizada |                     |                        |                    | X                          |                         |                         |                            |                       |                       |
| RF05 - Sistema de Favoritos                    |                     |                        |                    |                            | X                       |                         |                            |                       |                       |
| RF06 - Comunidade e Fóruns                     |                     |                        |                    |                            |                         | X                       |                            |                       |                       |
| RF07 - Envio de Notificações                   |                     |                        |                    |                            |                         |                         | X                          |                       |                       |
| RF08 - Coleta e Análise de Feedback            |                     |                        |                    |                            |                         |                         |                            | X                     |                       |
| RF09 - Suporte via tutoriais e tickets         |                     |                        |                    |                            |                         |                         |                            |                       | X                     |

### 2.4 Requisitos x Requisitos (Dependências)

| Requisito                                    | RF01 | RF02 | RF03 | RF04 | RF05 | RF06 | RF07 | RF08 | RF09 |
| :------------------------------------------- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| RF01 - Login de Usuário                       | -    |      |      |      |      |      |      |      |      |
| RF02 - Cadastro de Usuário                    |      | -    |      |      |      |      |      |      |      |
| RF03 - Acesso ao Feed de Notícias             |      |      | -    |      |      |      |      |      |      |
| RF04 - Sistema de Documentação Personalizada |      |      |      | -    |      |      |      |      |      |
| RF05 - Sistema de Favoritos                    |      |      |      |      | -    |      |      |      |      |
| RF06 - Comunidade e Fóruns                     |      |      |      |      |      | -    |      |      |      |
| RF07 - Envio de Notificações                   |      |      |      |      |      |      | -    |      |      |
| RF08 - Coleta e Análise de Feedback            |      |      |      |      |      |      |      | -    |      |
| RF09 - Suporte via tutoriais e tickets         |      |      |      |      |      |      |      |      | -    |

---

## 3. Análise de Impacto

O processo para análise de impacto de mudanças nos requisitos da plataforma educacional online "Tá na Mão" é o seguinte:

1.  Identificar o requisito a ser alterado.
2.  Consultar a matriz de rastreabilidade para verificar todos os casos de uso, componentes e casos de teste relacionados ao requisito.
3.  Avaliar o impacto da mudança em cada elemento relacionado.
4.  Documentar a análise de impacto.
5.  Obter aprovação da equipe responsável e stakeholders para a mudança.
6.  Atualizar todos os artefatos do projeto afetados pela alteração.

>[!IMPORTANT]
>A matriz de rastreabilidade deve ser mantida atualizada durante todo o ciclo de desenvolvimento para garantir a integridade do sistema e facilitar a gestão de mudanças.
>




docs/requisitos/documento_requisitos.md
