# ✅ **Checklist de Estudo: Spring Boot com Clean Architecture**

---

## 📘 Semana 1 – Fundamentos do Spring Boot

* [ ] Criar projeto com Spring Initializr
* [ ] Entender a estrutura padrão do projeto
* [ ] Executar uma aplicação simples com `@SpringBootApplication`
* [ ] Criar o primeiro `@RestController` com endpoint GET
* [ ] Usar `@Autowired` para injetar uma classe de serviço
* [ ] Aprender sobre `application.properties`
* [ ] Executar com `mvn spring-boot:run`

---

## 🌐 Semana 2 – API REST + Validações

* [ ] Criar endpoints CRUD com `@PostMapping`, `@PutMapping`, etc
* [ ] Usar `@RequestBody`, `@PathVariable` e `@RequestParam`
* [ ] Implementar validação com `@Valid` e anotações como `@NotNull`, `@Size`
* [ ] Usar `DTOs` para entrada e saída de dados
* [ ] Testar endpoints com Postman ou REST Client

---

## 🧩 Semana 3 – Padrão MVC

* [ ] Estudar o padrão **Model-View-Controller**
* [ ] Separar camadas: Controller, Service, Model
* [ ] Implementar exemplo com `@Controller` (opcional: `Thymeleaf`)
* [ ] Adaptar para `@RestController` com retorno JSON
* [ ] Entender a transição de MVC para REST

---

## 🗃️ Semana 4 – Banco de Dados com JPA

* [ ] Criar entidade com `@Entity`
* [ ] Criar `Repository` com `JpaRepository`
* [ ] Mapear relacionamentos: `@OneToMany`, `@ManyToOne`
* [ ] Usar `application.properties` ou `.env` para configurar banco
* [ ] Realizar operações básicas (CRUD) via JPA

---

## 🧯 Semana 5 – Tratamento de Erros + Boas Práticas

* [ ] Implementar `@ControllerAdvice` para exceções globais
* [ ] Criar classes de erro customizadas (`CustomException`)
* [ ] Retornar `ResponseEntity` com status apropriado
* [ ] Aplicar boas práticas: logs, separação de camadas, `@Service`
* [ ] Organizar mensagens e status HTTP corretamente

---

## 📢 Semana 6 – Eventos com Spring

* [ ] Criar eventos com `ApplicationEventPublisher`
* [ ] Criar `@EventListener` para escutar eventos
* [ ] Disparar eventos entre camadas (ex: após salvar entidade)
* [ ] Entender o propósito de eventos assíncronos

---

## ✉️ Semana 7 – Mensageria (RabbitMQ/Kafka)

* [ ] Configurar RabbitMQ ou Kafka localmente
* [ ] Criar `MessageProducer` e `MessageListener`
* [ ] Serializar e enviar DTOs como mensagens
* [ ] Consumir mensagens em outra classe ou serviço
* [ ] Testar com fila real ou mock

---

## 🧱 Semana 8 – Clean Architecture + Variáveis de Ambiente

* [ ] Separar o projeto em camadas:

  * [ ] `adapter/`, `application/`, `domain/`, `infrastructure/`
* [ ] Implementar interfaces e inversão de dependência
* [ ] Usar `@ConfigurationProperties` para ler variáveis de ambiente
* [ ] Externalizar configs com `.env`, `application.yml` ou propriedades do sistema
* [ ] Finalizar projeto com boas práticas de arquitetura

---

### 🏁 Projeto Final

* [ ] Refatorar código anterior aplicando Clean Architecture
* [ ] Criar uma aplicação de domínio (ex: gerenciamento de pedidos)
* [ ] Integrar banco, eventos e mensageria
* [ ] Organizar tudo em repositório no GitHub
* [ ] Documentar com README claro e exemplos de uso