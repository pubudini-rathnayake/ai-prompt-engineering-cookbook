# Few-Shot Prompting

Few-shot prompting provides the model with a small number of examples (shots) before asking it to perform the task. This guides the model toward the pattern you want.

---

## When to Use

- When zero-shot gives inconsistent results
- Custom output formats
- Domain-specific tasks
- Classification with specific label names

---

## Template

```
Here are some examples:

Input: [example 1 input]
Output: [example 1 output]

Input: [example 2 input]
Output: [example 2 output]

Input: [example 3 input]
Output: [example 3 output]

Now do the same for:
Input: [your actual input]
Output:
```

---

## Examples

### Sentiment Analysis

```
Here are some examples:

Input: "I love this product, it works perfectly!"
Output: POSITIVE

Input: "Terrible experience, would not recommend."
Output: NEGATIVE

Input: "It's okay, nothing special."
Output: NEUTRAL

Now classify this:
Input: "The delivery was fast but the item was damaged."
Output:
```

### JSON Extraction

```
Extract the name and city from each sentence and return as JSON.

Input: "John lives in New York."
Output: {"name": "John", "city": "New York"}

Input: "Sara moved to London last year."
Output: {"name": "Sara", "city": "London"}

Input: "Pubudini is based in Kandy."
Output:
```

---

## Tips

- Use 3–5 examples for best results
- Make sure examples cover edge cases
- Keep example format consistent
