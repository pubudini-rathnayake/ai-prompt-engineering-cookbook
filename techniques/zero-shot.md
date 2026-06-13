# Zero-Shot Prompting

Zero-shot prompting means asking the model to perform a task without giving it any examples. You rely purely on the model's pre-trained knowledge.

---

## When to Use

- Simple, well-defined tasks
- When you don't have example data
- Quick prototyping

---

## Template

```
[Clear instruction of what you want]
[Context if needed]
[Format you want the output in]
```

---

## Examples

### Text Classification

```
Classify the following customer review as Positive, Negative, or Neutral.

Review: "The product arrived on time but the quality was disappointing."

Respond with one word only: Positive, Negative, or Neutral.
```

### Summarization

```
Summarize the following paragraph in exactly two sentences:

[paste your paragraph here]
```

### Language Detection

```
Detect the language of the following text and respond with the language name only.

Text: "ආයුබෝවන්, කොහොමද?"
```

---

## Tips

- Be as specific as possible about the output format
- State constraints clearly (word count, language, tone)
- If results are poor, switch to few-shot prompting
