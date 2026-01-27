# GameTester - Sistema de Gerenciamento de Testes de Jogos 🎮

Este projeto é uma aplicação web completa desenvolvida para a disciplina de **Desenvolvimento de Software para Web 1 (DSW1)** na **UFSCar**. O sistema tem como objetivo gerenciar sessões de testes, bugs e estratégias para projetos de jogos, contando com diferentes níveis de acesso e internacionalização.

## 🛠️ Tecnologias Utilizadas

- [cite_start]**Framework Principal:** [Spring Boot 3.5.3](https://spring.io/projects/spring-boot) [cite: 1]
- [cite_start]**Linguagem:** Java 17 [cite: 1]
- [cite_start]**Persistência de Dados:** Spring Data JPA / Hibernate [cite: 1]
- [cite_start]**Base de Dados:** PostgreSQL 
- [cite_start]**Segurança:** Spring Security (Controle de acesso por perfis) [cite: 1]
- [cite_start]**Template Engine:** Thymeleaf (com Spring Security Extras) [cite: 1]
- [cite_start]**Outros:** Validação de dados (Bean Validation) e agendamento de tarefas (@EnableScheduling) 

## 🏗️ Arquitetura e Funcionalidades

A aplicação segue o padrão **MVC (Model-View-Controller)** e inclui:

- **Controle de Acessos:** Diferenciação entre administradores e testadores.
- **Gerenciamento de Entidades:** Cadastro e manutenção de Usuários, Projetos, Estratégias de Teste e Bugs.
- **Internacionalização (i18n):** Suporte nativo para múltiplos idiomas (Português/Inglês).
- [cite_start]**Upload de Ficheiros:** Sistema para armazenamento de evidências (ex: imagens de bugs)[cite: 2].
- [cite_start]**Agendamento:** Execução de tarefas programadas via Spring Scheduling[cite: 3].

## 🚀 Como Executar

### Pré-requisitos
- JDK 17
- Maven 3+
- PostgreSQL instalado e em execução

### Configuração da Base de Dados
1. [cite_start]Crie uma base de dados no PostgreSQL chamada `sistema_testes_db`[cite: 2].
2. [cite_start]Configure o ficheiro `src/main/resources/application.properties` com as suas credenciais locais[cite: 2]:
   ```properties
   spring.datasource.username=seu_usuario
   spring.datasource.password=sua_senha
