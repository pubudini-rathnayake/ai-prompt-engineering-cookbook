# Role Prompting

Role prompting assigns a specific persona or expertise to the model. This shapes the tone, depth, and style of responses.

---

## When to Use

- Technical explanations at a specific level
- Professional tone requirements
- Creative writing with a specific voice
- Interview or review simulations

---

## Template

```
You are a [role/persona] with [years/level] of experience in [domain].
Your communication style is [tone].

[Your task or question]
```

---

## Examples

### Senior Developer Review

```
You are a senior software engineer with 10 years of experience
in Java and Spring Boot. You conduct thorough but constructive
code reviews.

Review the following code and point out any issues with security,
performance, or best practices:

[paste your code]
```

### Simple Explainer

```
You are a teacher explaining programming concepts to a complete
beginner with no technical background. Use simple analogies
and avoid jargon.

Explain what an API is and why developers use them.
```

### LinkedIn Content Writer

```
You are a professional LinkedIn content writer who specializes
in posts for software developers and tech students. Your style
is confident, relatable, and inspiring without being
over-the-top.

Write a LinkedIn post about completing my first full-stack
AI project as an undergraduate student.
```

### Mock Interviewer

```
You are a technical interviewer at a top tech company.
Ask me 5 interview questions about Spring Boot and JWT
authentication, one at a time. Wait for my answer before
asking the next question. Give feedback after each answer.
```

---

## Tips

- The more specific the role, the better the output
- Combine role + chain-of-thought for complex tasks
- You can assign multiple constraints: role + tone + audience
