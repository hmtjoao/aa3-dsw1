# GameTester - Sistema de Gerenciamento de Testes de Jogos 🎮

Este projeto é uma aplicação web completa desenvolvida para a disciplina de **Desenvolvimento de Software para Web 1 (DSW1)** na **UFSCar**. O sistema tem como objetivo gerenciar sessões de testes, bugs e estratégias para projetos de jogos, contando com diferentes níveis de acesso e internacionalização.

## 🛠️ Tecnologias Utilizadas

- **Framework Principal:** [Spring Boot 3.5.3](https://spring.io/projects/spring-boot)
- **Linguagem:** Java 17 
- **Persistência de Dados:** Spring Data JPA / Hibernate 
- **Base de Dados:** PostgreSQL 
- **Segurança:** Spring Security (Controle de acesso por perfis) 
- **Template Engine:** Thymeleaf (com Spring Security Extras) 
- **Outros:** Validação de dados (Bean Validation) e agendamento de tarefas (@EnableScheduling) 

## 🏗️ Arquitetura e Funcionalidades

A aplicação segue o padrão **MVC (Model-View-Controller)** e inclui:

- **Controle de Acessos:** Diferenciação entre administradores e testadores.
- **Gerenciamento de Entidades:** Cadastro e manutenção de Usuários, Projetos, Estratégias de Teste e Bugs.
- **Internacionalização (i18n):** Suporte nativo para múltiplos idiomas (Português/Inglês).
- **Upload de Ficheiros:** Sistema para armazenamento de evidências (ex: imagens de bugs).
- **Agendamento:** Execução de tarefas programadas via Spring Scheduling.

## 🚀 Como Executar

### Pré-requisitos
- JDK 17
- Maven 3+
- PostgreSQL instalado e em execução

### Configuração da Base de Dados
1. Crie uma base de dados no PostgreSQL chamada `sistema_testes_db`.
2. Configure o ficheiro `src/main/resources/application.properties` com as suas credenciais locais:
   ```properties
   spring.datasource.username=seu_usuario
   spring.datasource.password=sua_senha
