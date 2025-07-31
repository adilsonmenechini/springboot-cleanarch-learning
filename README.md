# 🗓️ Plano Completo de Estudo – Spring Boot + API + MVC + Eventos + Mensageria + Clean Architecture

---

## 🎯 Objetivo

Desenvolver um projeto completo e profissional usando Spring Boot, com foco em:

* APIs REST e padrão MVC
* Eventos no Spring Boot
* Mensageria com Kafka ou RabbitMQ
* Uso correto de variáveis de ambiente
* Aplicação da Clean Architecture para organizar o código
* Boas práticas, testes e deploy

---

## 📆 Cronograma Semanal

### [Checklist](checklist.md)
---

### Semana 1: Fundamentos do Spring Boot

* Conceitos: Spring Boot, IoC, DI (`@Autowired`), estrutura básica
* Prática: Criar app básico com `@RestController` e endpoint `GET`
* Anotações principais:
  `@SpringBootApplication`, `@RestController`, `@Autowired`, `@GetMapping`

---

### Semana 2: APIs REST e Validações

* Conceitos: Métodos HTTP, DTOs, validação (`@Valid`), camadas Controller/Service/Repository
* Prática: CRUD básico (Usuário/Pedido), testado com Postman
* Anotações:
  `@PostMapping`, `@PutMapping`, `@DeleteMapping`, `@RequestBody`,
  `@PathVariable`, `@RequestParam`, `@Valid`, `@NotNull`, `@Email`

---

### Semana 3: Padrão MVC com Spring Boot

* Conceitos:
  Padrão Model-View-Controller, separação Model, View, Controller
  Diferenças entre `@Controller` e `@RestController`
* Prática:
  Criar recurso com camadas Model, Service e Controller
  (Opcional: criar página com Thymeleaf)
* Anotações:
  `@Controller`, `@RestController`, `@ModelAttribute`, `@Service`, `@Repository`

---

### Semana 4: Banco de Dados com Spring Data JPA

* Conceitos: JPA, Hibernate, entidades e relacionamentos
* Prática: Configurar banco H2/PostgreSQL, criar entidades e persistir dados
* Anotações:
  `@Entity`, `@Id`, `@GeneratedValue`, `@ManyToOne`, `@JoinColumn`

---

### Semana 5: Tratamento de Erros e Boas Práticas

* Conceitos:
  Arquitetura em camadas, tratamento global de exceções
* Prática: Criar handlers globais com `@ControllerAdvice`, DTOs de erro, mensagens claras
* Anotações:
  `@ControllerAdvice`, `@ExceptionHandler`, `@ResponseStatus`

---

### Semana 6: Eventos no Spring Boot

* Conceitos:
  Event-driven design, `ApplicationEventPublisher`, eventos síncronos e assíncronos
* Prática: Criar evento ao criar recurso, listener com `@EventListener`
* Anotações:
  `@EventListener`, `@ApplicationEvent`, `@Async`, `@EnableAsync`

---

### Semana 7: Mensageria com Kafka ou RabbitMQ

* Conceitos:
  Produtores, consumidores, filas/tópicos, diferenças RabbitMQ vs Kafka
* Prática: Instalar via Docker, criar produtor e consumidor no Spring Boot
* Anotações:
  `@KafkaListener`, `@EnableKafka`, `@RabbitListener`, `@EnableRabbit`, `@SendTo`

---

### Semana 8: Integração Completa + Variáveis de Ambiente + Clean Architecture

* Conceitos:
  Externalizar configurações via `.env`, `application.yml`, `@Value`, `@ConfigurationProperties`
  Princípios da Clean Architecture: domínio isolado, casos de uso, inversão de dependência
* Prática:
  Integrar API, eventos e mensageria em projeto estruturado com camadas limpas
  Usar variáveis de ambiente para senhas, URLs, etc
  Docker Compose para orquestrar API, banco e broker
* Anotações:
  `@Value`, `@ConfigurationProperties`, `@Bean`

---

## 📦 Projeto Final Sugerido

**Sistema de Pedidos** com:

* API REST para criar e listar pedidos
* Evento `PedidoCriadoEvent` disparado ao criar pedido
* Mensagem publicada em Kafka ou RabbitMQ
* Consumidor que processa mensagem (log, notificação simulado)
* Estruturação em Clean Architecture (pastas e código)
* Configurações via variáveis de ambiente
* Testes unitários básicos
* Docker Compose para rodar tudo junto

---

## 📌 Tecnologias e Ferramentas Usadas

* Java 17+
* Spring Boot 3+
* Spring Data JPA + PostgreSQL/H2
* Kafka ou RabbitMQ (Docker)
* Lombok (opcional)
* MapStruct (opcional)
* JUnit + Mockito
* Docker + Docker Compose
* dotenv-java para carregar `.env` (opcional)

---

## Extensões recomendadas para VS Code

### 1. **Java Extension Pack** (Microsoft)

Pacote essencial que inclui:

* Language Support for Java™ by Red Hat
* Debugger for Java
* Java Test Runner
* Maven for Java
* Project Manager for Java

### 2. **Spring Boot Extension Pack** (Pivotal / Microsoft)

Inclui várias ferramentas úteis para Spring Boot:

* Spring Boot Tools
* Spring Initializr Java Support (para criar projetos facilmente)
* Spring Boot Dashboard (para gerenciar aplicações)
* Spring Boot Properties Support (ajuda com `application.properties` e `application.yml`)

### 3. **Docker** (Microsoft)

Para gerenciar containers Docker direto do VS Code.

### 4. **Lombok Annotations Support for VS Code**

Se usar Lombok para reduzir boilerplate.

### 5. **YAML** (Red Hat)

Para editar arquivos `application.yml` com suporte a sintaxe e autocomplete.

### 6. **REST Client** (Huachao Mao)

Para testar suas APIs REST diretamente no VS Code, sem precisar usar Postman.