# 🐍 Python Senior Knowledge Base

> Deep dive em Python, Django, FastAPI, databases e arquitetura para nível senior

[![Python](https://img.shields.io/badge/Python-3.11+-blue.svg)](https://www.python.org/downloads/)
[![Django](https://img.shields.io/badge/Django-5.0+-green.svg)](https://www.djangoproject.com/)
[![FastAPI](https://img.shields.io/badge/FastAPI-0.104+-teal.svg)](https://fastapi.tiangolo.com/)

---

## 📚 Estrutura do Repositório

```
.
├── python-internals/        # Python avançado
│   ├── gil.md
│   ├── memory-management.md
│   ├── async-await.md
│   ├── decorators.md
│   └── type-hints.md
├── django-deep-dive/        # Django expertise
│   ├── orm-optimization.md
│   ├── middleware.md
│   ├── async-views.md
│   └── security.md
├── fastapi-mastery/         # FastAPI profundo
│   ├── dependency-injection.md
│   ├── async-patterns.md
│   └── testing.md
├── databases/               # PostgreSQL, Redis, MongoDB
│   ├── postgresql.md
│   ├── redis.md
│   └── query-optimization.md
├── architecture/            # Patterns e design
│   ├── microservices.md
│   ├── caching-strategies.md
│   └── api-design.md
├── testing/                 # Testing best practices
├── devops/                  # Docker, CI/CD
├── examples/                # Código de exemplo
└── flashcards/             # Flashcards para Anki
```

---

## 🎯 Roadmap de Estudo (Semanas 5-6)

### Semana 5: Python & Frameworks

#### Dia 1 (05/11) - Python Internals
- [ ] GIL (Global Interpreter Lock)
- [ ] Memory management & garbage collection
- [ ] Decorators avançados
- [ ] Generators & iterators
- [ ] async/await & asyncio
- [ ] 📝 **30 flashcards**

#### Dia 2 (06/11) - Python Performance & Type Hints
- [ ] Profiling (cProfile, line_profiler, memory_profiler)
- [ ] `__slots__`, list comprehension vs generators
- [ ] Type hints avançados (Protocol, TypeVar, Generic, ParamSpec)
- [ ] Python 3.10+ features (match/case, union types)
- [ ] 📝 **25 flashcards**

#### Dia 3 (07/11) - Django Deep Dive Part 1
- [ ] ORM avançado (select_related, prefetch_related, annotate)
- [ ] Query optimization, índices, database routers
- [ ] Middleware customizado, signals, custom managers
- [ ] QuerySet lazy evaluation
- [ ] 📝 **30 flashcards**

#### Dia 4 (08/11) - Django Deep Dive Part 2
- [ ] Async views, Django Channels, WebSockets
- [ ] Security (CSRF, XSS, SQL injection, clickjacking)
- [ ] Caching strategies (Redis, Memcached, database cache)
- [ ] Celery integration, background tasks
- [ ] 📝 **30 flashcards**

#### Dia 5 (11/11) - FastAPI Mastery
- [ ] Dependency injection profundo
- [ ] Background tasks, WebSockets, Server-Sent Events
- [ ] Async best practices, conexões de database
- [ ] Testing com pytest-asyncio
- [ ] Django vs FastAPI - quando usar cada um
- [ ] 📝 **25 flashcards**

### Semana 6: Databases & Architecture

#### Dia 6 (12/11) - PostgreSQL Deep Dive
- [ ] Índices (B-tree, Hash, GiST, GIN, BRIN)
- [ ] Query optimization, EXPLAIN ANALYZE
- [ ] Partitioning (range, list, hash)
- [ ] Replication, sharding concepts
- [ ] ACID, isolation levels, transactions
- [ ] 📝 **30 flashcards**

#### Dia 7 (13/11) - NoSQL & Caching
- [ ] Redis data structures & use cases
- [ ] MongoDB: aggregation pipeline, indexing
- [ ] CAP theorem, eventual consistency
- [ ] SQL vs NoSQL - quando usar
- [ ] Cache patterns (cache-aside, write-through, write-behind)
- [ ] 📝 **25 flashcards**

#### Dia 8 (14/11) - APIs & Microservices
- [ ] REST best practices, API versioning
- [ ] GraphQL basics
- [ ] Rate limiting strategies
- [ ] Service discovery, circuit breaker pattern
- [ ] API Gateway pattern
- [ ] 📝 **25 flashcards**

#### Dia 9 (15/11) - Testing & DevOps
- [ ] Unit, integration, e2e tests
- [ ] Mocking, fixtures, parametrize (pytest)
- [ ] TDD philosophy, test pyramid
- [ ] Docker basics, docker-compose
- [ ] CI/CD concepts (GitHub Actions)
- [ ] 📝 **20 flashcards**

---

## 📊 Progresso

```
Tópicos Estudados: 0/40+ (0%)
Flashcards Criados: 0/250+ (0%)
Exemplos de Código: 0/20 (0%)
Mock Interviews: 0/2 (0%)
```

**Meta:** 250+ flashcards até final da Semana 6

---

## 🎴 Sistema de Flashcards

### Como Usar

1. **Durante o estudo:** Criar flashcards em `flashcards/`
2. **Formato:** Um arquivo por tópico
3. **Review:** Usar Anki ou similar
4. **Frequência:** Review diário de 50-100 cards

### Estrutura de um Flashcard

```
Q: O que é GIL no Python?
A: Global Interpreter Lock - um mutex que protege acesso a objetos Python,
   prevenindo múltiplas threads de executar bytecode Python simultaneamente.
   Impact: Limita paralelismo em programas CPU-bound multi-threaded.
   Alternativas: multiprocessing, asyncio para I/O-bound
Tags: python, internals, concurrency
```

---

## 💻 Exemplos de Código

Cada tópico importante terá código de exemplo em `examples/`:

```
examples/
├── async-patterns/
│   ├── asyncio_basics.py
│   ├── concurrent_requests.py
│   └── async_context_manager.py
├── django-optimization/
│   ├── query_optimization.py
│   ├── custom_middleware.py
│   └── celery_tasks.py
└── fastapi-patterns/
    ├── dependency_injection.py
    ├── background_tasks.py
    └── websockets.py
```

---

## 🎯 Tópicos Principais

### Python Internals

<details>
<summary><b>Clique para expandir</b></summary>

#### GIL (Global Interpreter Lock)
- O que é e por que existe
- Impact em multi-threading
- Quando é released
- Alternativas (multiprocessing, asyncio)
- GIL-free Python proposals

#### Memory Management
- Reference counting
- Garbage collection (generational)
- Memory pools
- `__del__` e finalizers
- Memory profiling

#### Async/Await
- Event loop internals
- Coroutines vs generators
- asyncio primitives (Task, Future, gather, wait)
- Async context managers e iterators
- Common pitfalls

#### Decorators
- Function decorators
- Class decorators
- Decorators com argumentos
- functools.wraps
- Use cases (caching, logging, auth)

#### Type Hints
- Basic types
- Generic types (List, Dict, Optional)
- Protocol (structural subtyping)
- TypeVar e Generic classes
- ParamSpec e Concatenate
- Runtime type checking

</details>

### Django Deep Dive

<details>
<summary><b>Clique para expandir</b></summary>

#### ORM Optimization
- select_related vs prefetch_related
- only() e defer()
- annotate() e aggregate()
- F() e Q() objects
- Raw SQL quando necessário
- Database indexes

#### Middleware
- Request/response cycle
- Custom middleware
- Order matters
- Common middleware patterns

#### Async Django
- Async views
- ASGI vs WSGI
- Django Channels
- WebSockets
- When to use async

#### Security
- CSRF protection
- XSS prevention
- SQL injection
- Clickjacking protection
- CORS
- Authentication & Authorization

</details>

### FastAPI Mastery

<details>
<summary><b>Clique para expandir</b></summary>

#### Dependency Injection
- Depends() function
- Security dependencies
- Database dependencies
- Request/response dependencies
- Testing with overrides

#### Async Patterns
- Async route handlers
- Background tasks
- WebSockets
- Server-Sent Events
- Database connections (async)

#### Advanced Features
- Custom response classes
- Middleware
- Exception handlers
- Request validation
- Response model

</details>

### Database Expertise

<details>
<summary><b>Clique para expandir</b></summary>

#### PostgreSQL
- Index types e quando usar
- EXPLAIN ANALYZE
- Query optimization
- Partitioning strategies
- Replication
- Connection pooling

#### Redis
- Data structures (String, Hash, List, Set, Sorted Set)
- Use cases (cache, session, queue, pub/sub)
- Persistence (RDB vs AOF)
- Clustering
- Memory optimization

#### NoSQL
- MongoDB basics
- When to use NoSQL vs SQL
- CAP theorem
- Eventual consistency

</details>

---

## 🚀 Como Usar Este Repositório

### Setup

```bash
git clone https://github.com/seu-username/python-senior-knowledge.git
cd python-senior-knowledge

# Instalar dependências para exemplos
pip install -r requirements.txt
```

### Estudar um Tópico

1. Ler o arquivo `.md` do tópico
2. Executar exemplos em `examples/`
3. Criar flashcards para conceitos importantes
4. Fazer anotações pessoais
5. Praticar explicando em voz alta

### Adicionar Novo Conteúdo

```bash
# Criar novo arquivo de notas
touch python-internals/novo-topico.md

# Adicionar exemplo
mkdir examples/novo-topico
touch examples/novo-topico/example.py

# Commit
git add .
git commit -m "docs(python): add notes on novo-topico"
git push
```

---

## 📖 Recursos Externos

### Livros
- [Fluent Python](https://www.oreilly.com/library/view/fluent-python-2nd/9781492056348/) - Luciano Ramalho
- [High Performance Python](https://www.oreilly.com/library/view/high-performance-python/9781492055013/)
- [Two Scoops of Django](https://www.feldroy.com/books/two-scoops-of-django-3-x)

### Online
- [Real Python](https://realpython.com/)
- [Python's official docs](https://docs.python.org/3/)
- [Django documentation](https://docs.djangoproject.com/)
- [FastAPI documentation](https://fastapi.tiangolo.com/)

### Vídeos
- [ArjanCodes - Python](https://www.youtube.com/c/ArjanCodes)
- [mCoding - Advanced Python](https://www.youtube.com/c/mCoding)

---

## 💡 Metodologia de Estudo

### Para Cada Tópico (4 horas):

1. **Leitura ativa** (1.5h)
   - Ler documentação oficial
   - Anotar conceitos principais
   - Identificar dúvidas

2. **Prática** (1.5h)
   - Escrever código de exemplo
   - Testar edge cases
   - Comparar alternativas

3. **Consolidação** (1h)
   - Criar flashcards (20-30)
   - Explicar em voz alta
   - Conectar com conhecimento anterior

---

## 🎤 Mock Interviews Técnicas

### Mock 1 (11/11 - Final Semana 5)
- [ ] Python: GIL, async, decorators (10min)
- [ ] Django/FastAPI questions (10min)
- [ ] Databases (10min)
- [ ] Coding: 1 problema DP (30min)

### Mock 2 (18/11 - Semana 7)
- [ ] Review completo de todos tópicos
- [ ] Perguntas aleatórias
- [ ] Gravar e analisar

---

## 📝 Notas

Este repositório documenta o conhecimento técnico adquirido durante as Semanas 5-6 do plano de estudos (04/11 - 15/11/2025). Foco em profundidade técnica para posições senior backend.

---

## 📫 Contribuições

Este é um repositório pessoal de estudo, mas sugestões são bem-vindas via [issues](https://github.com/seu-username/python-senior-knowledge/issues)!

---

**Status:** 🚧 Início previsto para 05/11/2025  
**Meta:** 250+ flashcards + exemplos práticos
