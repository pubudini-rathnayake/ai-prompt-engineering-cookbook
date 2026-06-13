# Structured Output Prompting

Structured output prompting instructs the model to return data in a specific format such as JSON, Markdown tables, bullet lists, or XML. Essential for building AI-powered applications.

---

## When to Use

- Parsing AI responses in code
- Building RAG pipelines
- Data extraction tasks
- Generating content for UI components

---

## Templates

### JSON Output

```
Extract the following information from the text below and return
it as a valid JSON object only. Do not include any explanation
or markdown formatting.

Fields to extract:
- name (string)
- email (string)
- skills (array of strings)

Text:
[paste your text]
```

### Markdown Table

```
Compare [Topic A] and [Topic B] across the following dimensions:
[dimension 1], [dimension 2], [dimension 3].

Return your response as a Markdown table only.
```

### Numbered Steps

```
Provide a step-by-step guide for [task].
Format your response as a numbered list.
Each step should be one sentence maximum.
```

---

## Examples

### Resume Parser

```
Extract structured data from the resume text below.
Return ONLY a valid JSON object with no extra text.

{
  "name": "",
  "email": "",
  "education": [],
  "skills": [],
  "experience": []
}

Resume:
[paste resume text here]
```

### RAG System Prompt

```
You are a helpful assistant. Answer the user's question using
ONLY the context provided below. If the answer is not in the
context, respond with: "I don't have enough information."

Return your answer in this JSON format only:
{
  "answer": "",
  "confidence": "high | medium | low",
  "source_used": true | false
}

Context:
[retrieved context here]

Question:
[user question here]
```

---

## Tips

- Always say "Return ONLY JSON" to prevent extra text
- Validate parsed JSON in your application code
- Use Pydantic or Zod for schema validation on the output
