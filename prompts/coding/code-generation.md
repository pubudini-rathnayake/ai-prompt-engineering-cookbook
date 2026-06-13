# Code Generation Prompts

Prompts to generate clean, production-ready code.

---

## REST API Endpoint

```
Generate a [language] [framework] REST API endpoint with
the following specifications:

Method: [GET/POST/PUT/DELETE]
Path: [/api/...]
Request body: [describe fields]
Response: [describe response]
Validation: [list validation rules]
Error handling: [describe error cases]

Follow best practices and include comments.
```

---

## Database Entity / Model

```
Generate a [Spring Boot JPA Entity / Django Model / Mongoose Schema]
for the following:

Entity name: [name]
Fields:
- [field name]: [type], [constraints]
- [field name]: [type], [constraints]

Relationships:
- [describe any relationships]

Include proper annotations and follow naming conventions.
```

---

## LangChain RAG Chain

```
Generate a Python LangChain RAG chain with the following:

Vector store: ChromaDB
Embedding model: Google Gemini (gemini-embedding-001)
LLM: Gemini 2.5 Flash Lite
Retrieval: Top 4 most relevant chunks
Prompt: Custom prompt that answers only from context

Include error handling and comments explaining each step.
```

---

## Unit Test

```
Generate unit tests for the following [language] function/class.

Code to test:
[paste your code]

Cover these cases:
- Happy path
- Edge cases
- Error/exception cases

Use [JUnit 5 / pytest / Jest] and follow AAA pattern
(Arrange, Act, Assert).
```
