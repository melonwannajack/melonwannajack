# Software Engineering — Plan de estudios vivo

## 0. Meta-capa: qué significa saber ingeniería del software

- modelar problemas
- construir sistemas mantenibles
- razonar sobre coste, complejidad y fallo
- operar software en producción
- comunicar decisiones técnicas
- trabajar con restricciones reales

---

## 1. Computer Science Foundations

### 1.1. Lógica, matemáticas discretas y modelos de computación
- lógica proposicional y de predicados
- conjuntos, relaciones y funciones
- inducción y recursión
- combinatoria básica
- grafos
- autómatas y lenguajes formales
- computabilidad
- decidibilidad
- complejidad computacional

### 1.2. Qué debería saber hacer
- demostrar corrección básica de algoritmos
- razonar con invariantes
- distinguir problema decidible / tratable / eficiente
- ver un programa como objeto matemático, no solo como artefacto práctico

### 1.3. Pendientes típicos
- teoría de autómatas
- reducibilidad
- NP-completitud con soltura

---

## 2. Programming as a Discipline

### 2.1. Programación como traducción de modelos
- especificación vs implementación
- semántica informal y formal
- tipos como restricción y documentación
- invariantes de datos
- contratos
- precondiciones / postcondiciones

### 2.2. Paradigmas
- procedural
- structured programming
- object-oriented programming
- functional programming
- declarative programming
- event-driven programming
- reactive programming
- data-oriented design

### 2.3. Temas profundos
- mutabilidad vs inmutabilidad
- identidad vs valor
- composición
- efectos secundarios
- closures
- dispatch
- polimorfismo
- genericidad
- type systems
- error handling
- async as control-flow model

### 2.4. Qué debería saber hacer
- elegir paradigma según problema
- detectar cuándo OOP complica más de lo que ayuda
- usar funciones puras donde mejoran testabilidad
- modelar dominio con tipos y no solo con comentarios
- separar lógica de negocio, IO y coordinación

---

## 3. Algorithms

### 3.1. Fundamentos
- análisis de complejidad
- notación O, Ω, Θ
- coste temporal amortizado
- coste espacial
- recursión
- recurrencias
- estabilidad
- optimalidad

### 3.2. Familias clásicas
- sorting
  - insertion
  - merge
  - quick
  - heap
  - radix / counting
- searching
  - linear
  - binary
  - indexed lookup
- divide and conquer
- greedy
- dynamic programming
- backtracking
- branch and bound
- randomized algorithms

### 3.3. Algoritmos sobre grafos
- BFS / DFS
- topological sort
- connected components
- shortest paths
  - Dijkstra
  - Bellman-Ford
  - Floyd-Warshall
- spanning trees
- max flow / min cut
- matching
- SCC

### 3.4. Algoritmos sobre strings y secuencias
- hashing
- KMP
- suffix arrays / trees
- edit distance
- rolling hashes
- parsing básico

### 3.5. Qué debería saber hacer
- escoger estructura + algoritmo conjuntamente
- justificar una elección por complejidad y contexto real
- detectar cuellos de botella algorítmicos
- reconocer cuándo una mejora micro no compensa una mala estrategia

---

## 4. Data Structures

### 4.1. Lineales
- arrays
- dynamic arrays
- linked lists
- stacks
- queues
- deques

### 4.2. Associative
- hash tables
- ordered maps
- sets
- multisets

### 4.3. Arbóreas
- BST
- AVL / Red-Black Trees
- heaps
- B-trees / B+ trees
- tries

### 4.4. Especializadas
- union-find
- segment tree
- Fenwick tree
- interval tree
- bloom filter
- LRU / LFU structures

### 4.5. Qué debería saber hacer
- entender representación física y coste real
- relacionar estructura con locality of reference
- distinguir complejidad teórica de rendimiento observado
- elegir estructuras según lectura/escritura/orden/persistencia

---

## 5. Compilers, Interpreters and Language Runtime

### 5.1. Lenguajes como sistemas
- lexical analysis
- parsing
- AST
- semantic analysis
- type checking
- bytecode / IR
- interpretation vs compilation
- JIT vs AOT

### 5.2. Runtime
- stack vs heap
- closures
- garbage collection
- reference counting
- memory ownership
- exception machinery

### 5.3. Qué debería saber hacer
- entender qué hace realmente el runtime del lenguaje que usa
- razonar sobre coste de abstracciones
- leer errores de compilación desde el modelo interno del lenguaje

---

## 6. Operating Systems

### 6.1. Procesos y concurrencia
- processes
- threads
- context switching
- scheduling
- synchronization
- mutexes
- semaphores
- condition variables
- deadlocks
- race conditions

### 6.2. Memoria
- virtual memory
- paging
- segmentation
- memory allocation
- stack / heap
- cache hierarchy
- locality
- copy-on-write

### 6.3. IO y sistema
- syscalls
- files
- pipes
- sockets
- signals
- polling
- epoll / kqueue
- buffering

### 6.4. Kernel
- mode user / kernel
- interrupts
- device drivers
- scheduler
- VFS

### 6.5. Qué debería saber hacer
- entender qué ocurre cuando ejecutas un programa
- razonar sobre procesos, hilos y coste de coordinación
- distinguir CPU-bound, IO-bound y memory-bound
- depurar problemas de bloqueo, leaks y contention

---

## 7. Linux and Systems Practice

### 7.1. Entorno
- shell
- pipes
- redirections
- environment
- permissions
- users/groups
- package management
- systemd

### 7.2. Observación del sistema
- ps
- top / htop
- lsof
- strace
- tcpdump
- ss / netstat
- perf
- dmesg
- journald

### 7.3. Administración básica
- filesystem layout
- mounts
- services
- cron
- logs
- ulimits
- SSH
- containers

### 7.4. Qué debería saber hacer
- moverse con fluidez en un sistema Linux
- diagnosticar problemas simples de red, permisos, procesos y memoria
- tratar Linux como plataforma de trabajo y no como caja negra

---

## 8. Computer Architecture and Hardware

### 8.1. Modelo hardware
- CPU
- ALU
- registers
- instruction pipeline
- branch prediction
- superscalar execution
- SIMD
- multicore

### 8.2. Memoria
- cache L1/L2/L3
- RAM
- NUMA
- disk / SSD
- latency vs throughput

### 8.3. IO y buses
- interrupts
- DMA
- PCIe
- storage paths

### 8.4. Qué debería saber hacer
- entender por qué el acceso a memoria domina muchos programas
- ver cómo las decisiones de diseño de datos impactan caché y rendimiento
- distinguir paralelismo real de ilusión de concurrencia

---

## 9. Networking

### 9.1. Fundamentos
- OSI vs TCP/IP
- IP
- routing
- ARP
- DNS
- NAT
- ports

### 9.2. Transporte y aplicación
- TCP
- UDP
- handshakes
- retransmission
- congestion
- HTTP
- HTTP/2
- HTTP/3
- WebSocket
- gRPC

### 9.3. Sistemas distribuidos desde red
- latency
- retries
- timeouts
- backoff
- idempotency
- partial failure

### 9.4. Qué debería saber hacer
- seguir el camino conceptual de una request
- detectar dónde puede fallar una comunicación
- entender por qué la red convierte sistemas simples en distribuidos y frágiles

---

## 10. Databases and Storage

### 10.1. Modelado
- entidades y relaciones
- normalización
- constraints
- claves
- integridad

### 10.2. SQL profundo
- joins
- subqueries
- window functions
- CTEs
- execution plans
- indexing

### 10.3. Internals
- pages
- B-trees
- MVCC
- WAL
- locks
- transactions
- ACID
- isolation levels

### 10.4. NoSQL
- key-value
- document
- columnar
- graph
- trade-offs reales

### 10.5. Distribución
- replication
- partitioning
- sharding
- leader election
- eventual consistency

### 10.6. Qué debería saber hacer
- modelar datos para negocio y rendimiento
- leer un plan de ejecución
- elegir SQL o NoSQL por requisitos concretos, no por moda
- razonar sobre consistencia, concurrencia y recuperación

---

## 11. Software Architecture

### 11.1. Modos de estructurar sistemas
- monolith
- modular monolith
- microservices
- service-oriented architecture
- event-driven systems
- serverless
- batch systems

### 11.2. Fronteras
- bounded contexts
- interfaces
- contracts
- schema evolution
- backward compatibility

### 11.3. Problemas reales
- coupling
- cohesion
- dependency direction
- configuration
- deployment topology
- failure domains

### 11.4. Patrones
- layered architecture
- hexagonal architecture
- clean architecture
- ports & adapters
- repository
- unit of work
- outbox
- saga
- circuit breaker

### 11.5. Qué debería saber hacer
- explicar por qué una arquitectura concreta tiene sentido bajo ciertas restricciones
- distinguir modularidad conceptual de simple separación en carpetas
- entender que microservicios introducen complejidad operativa, organizativa y de datos

---

## 12. Distributed Systems

### 12.1. Conceptos base
- clocks
- ordering
- consensus
- replication
- coordination
- partitions
- leader election

### 12.2. Teoremas y límites
- CAP
- FLP
- consistency trade-offs
- quorum systems

### 12.3. Práctica
- queues
- logs
- stream processing
- retries
- deduplication
- idempotency
- message ordering
- exactly-once as marketing claim

### 12.4. Qué debería saber hacer
- razonar sobre fallo parcial
- diseñar sistemas que toleren reintentos y duplicados
- entender que la complejidad distribuida nace del desacoplamiento temporal y de la red

---

## 13. API Design and Integration

### 13.1. Diseño
- resources vs actions
- versioning
- pagination
- filtering
- validation
- error modeling
- idempotency keys

### 13.2. Contratos
- OpenAPI
- schema-first
- backward compatibility
- consumer-driven contracts

### 13.3. Integración
- webhooks
- polling
- async callbacks
- eventual consistency across APIs

### 13.4. Qué debería saber hacer
- diseñar APIs previsibles
- evitar diseños acoplados al frontend del momento
- modelar errores como parte central del contrato

---

## 14. Frontend Engineering

### 14.1. Web platform
- HTML semantics
- CSS cascade
- layout
- accessibility
- browser rendering pipeline
- event loop

### 14.2. JavaScript / TypeScript profundo
- closures
- prototypes
- async/await
- promises
- module systems
- type narrowing
- generics

### 14.3. Arquitectura frontend
- state
- server state vs client state
- rendering models
- hydration
- routing
- forms
- design systems
- atomic design

### 14.4. Performance
- bundle size
- caching
- code splitting
- rendering cost
- memoization
- network waterfalls

### 14.5. Qué debería saber hacer
- distinguir problemas de UI, estado, red y rendering
- modelar un frontend como sistema y no como colección de componentes
- pensar en accesibilidad y rendimiento desde el diseño

---

## 15. Backend Engineering

### 15.1. Application design
- request lifecycle
- dependency injection
- configuration management
- background jobs
- transactional boundaries

### 15.2. Concurrency and scaling
- worker pools
- queues
- rate limits
- caches
- horizontal scaling
- statelessness

### 15.3. Reliability
- retries
- timeouts
- bulkheads
- graceful degradation
- backpressure

### 15.4. Qué debería saber hacer
- construir servicios legibles y operables
- aislar dominio, aplicación e infraestructura
- tratar concurrencia y observabilidad como partes del diseño, no añadidos

---

## 16. Security Engineering

### 16.1. Fundamentos
- confidentiality
- integrity
- availability
- threat modeling
- trust boundaries
- least privilege

### 16.2. Aplicación
- authn vs authz
- sessions
- OAuth / OIDC
- secrets management
- input validation
- output encoding
- CSRF
- XSS
- SSRF
- SQL injection

### 16.3. Infraestructura
- TLS
- key management
- certificates
- hardening
- secure deployment

### 16.4. Práctica ofensiva y defensiva
- pentesting básico
- vulnerability scanning
- dependency risk
- incident response

### 16.5. Qué debería saber hacer
- pensar como atacante al diseñar flujos
- identificar superficies de ataque
- comprender que seguridad es propiedad sistémica, no checklist

---

## 17. Testing and Verification

### 17.1. Niveles
- unit tests
- integration tests
- end-to-end tests
- contract tests
- property-based tests
- snapshot tests con criterio

### 17.2. Estrategia
- test pyramid
- test isolation
- fixtures
- mocks vs fakes
- determinism

### 17.3. Calidad
- static analysis
- linting
- type checking
- code review
- formal verification en casos críticos

### 17.4. Qué debería saber hacer
- decidir qué test aporta señal
- no confundir cobertura con confianza
- usar tipos, contratos y diseño para reducir necesidad de tests frágiles

---

## 18. DevOps, Delivery and Operations

### 18.1. Build and release
- build pipelines
- artifacts
- reproducibility
- CI/CD
- release strategies
- feature flags
- rollback

### 18.2. Infra
- containers
- Docker
- orchestration
- Kubernetes
- IaC
- networking in cloud
- storage in cloud

### 18.3. Operación
- logs
- metrics
- traces
- alerting
- SLO / SLA / SLI
- on-call
- incident review

### 18.4. Qué debería saber hacer
- desplegar con seguridad
- entender qué significa operar software de verdad
- observar un sistema y no solo “mirar logs”

---

## 19. Engineering Process and Collaboration

### 19.1. Workflow
- git deep usage
- branching models
- commit discipline
- code review
- RFCs / ADRs
- ticket refinement

### 19.2. Gestión
- agile como conjunto de heurísticas, no ritual
- kanban
- planning
- estimation
- prioritization
- technical debt
- roadmap

### 19.3. Comunicación
- documentación
- arquitectura explicada
- incident reports
- design docs
- mentoring

### 19.4. Qué debería saber hacer
- escribir para que otros puedan continuar el trabajo
- convertir decisiones implícitas en artefactos compartibles
- colaborar sin generar deuda comunicativa

---

## 20. Performance Engineering

### 20.1. Perfilado
- CPU profiling
- memory profiling
- IO profiling
- flame graphs

### 20.2. Niveles
- algorithmic performance
- data layout
- database performance
- network performance
- rendering performance

### 20.3. Qué debería saber hacer
- medir antes de optimizar
- identificar el nivel correcto del problema
- no optimizar microdetalles cuando el cuello es arquitectónico

---

## 21. Domain Modeling

### 21.1. Modelar antes de codificar
- lenguaje ubicuo
- entidades
- value objects
- aggregates
- invariants
- workflows
- temporalidad

### 21.2. Qué debería saber hacer
- distinguir complejidad accidental de complejidad del dominio
- construir software que refleje el problema y no solo la base de datos

---

## 22. Specialization tracks

### 22.1. Systems / Infrastructure
- OS profundo
- networking avanzado
- distributed systems
- performance
- kernel / compilers opcional

### 22.2. Backend / Platform
- APIs
- databases
- architecture
- queues
- observability
- cloud

### 22.3. Frontend / Product engineering
- browser internals
- state management
- accessibility
- performance
- design systems

### 22.4. Data / ML engineering
- data pipelines
- storage formats
- distributed compute
- feature serving
- model deployment
- reproducibility

### 22.5. Security
- offensive basics
- secure systems
- auth
- infra hardening
- appsec

---

## 23. Self-assessment model

Para cada tema:

- 0: no expuesto
- 1: conozco vocabulario
- 2: entiendo conceptos
- 3: lo aplico con ayuda
- 4: lo aplico solo
- 5: lo explico y diseño con criterio
- 6: detecto trade-offs y anti-patrones
- 7: puedo enseñar / revisar / liderar

---

## 24. Evidence of mastery

Cada bloque debería tener al menos una de estas pruebas:

- notas propias
- implementación pequeña
- bug real resuelto
- ejercicio de diseño
- postmortem de error
- benchmark
- mini proyecto
- lectura resumida
- comparación entre alternativas

---

## 25. Missing areas to complete later

### Formal CS
- compilers
- automata / PL theory
- computability / complexity

### Systems
- kernel internals
- scheduling
- memory deep dive
- network debugging real

### Distributed systems
- Raft / Paxos
- stream systems
- consistency models en práctica

### Security
- exploit classes
- secure architecture
- secrets and identity deep dive

### Operations
- observability madura
- SLOs
- incident response
- capacity planning
