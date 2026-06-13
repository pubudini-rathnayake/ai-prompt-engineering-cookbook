# Chain-of-Thought (CoT) Prompting

Chain-of-thought prompting encourages the model to reason step by step before giving a final answer. This dramatically improves accuracy on complex tasks.

---

## When to Use

- Math and logic problems
- Multi-step reasoning
- Complex decision making
- Debugging and root cause analysis

---

## Template

```
[Your question or problem]

Think through this step by step before giving your final answer.
```

---

## Examples

### Problem Solving

```
A student has 3 assignments due this week. Each takes 2 hours.
She also has a part-time job for 4 hours on two days.
She has 20 hours of free time total this week.
Will she have enough time to finish all assignments?

Think through this step by step before giving your final answer.
```

### Debugging

```
My FastAPI endpoint returns a 422 error when I send a POST request
with a JSON body. Here is my Pydantic model and route code:

[paste your code]

Think through the possible causes step by step and suggest a fix.
```

### Code Logic

```
Explain why this Python function returns the wrong output
for the input [1, 2, 3]:

def mystery(lst):
    result = []
    for i in range(len(lst)):
        result.append(lst[i] * i)
    return result

Walk through the execution step by step.
```

---

## Tips

- Add "Think step by step" or "Let's think through this" to trigger CoT
- Works best with GPT-4, Gemini 1.5+, and Claude 3+
- Combine with few-shot for even better results
