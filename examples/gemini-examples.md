# Google Gemini Prompt Examples

Real prompt examples tested with Google Gemini 2.5 Flash.

---

## Text Summarization

**Prompt:**

```
Summarize the following research paper abstract in 3 bullet points
for a general audience with no technical background:

[paste abstract]
```

**Works best with:** Gemini 1.5 Flash, Gemini 2.5 Flash Lite

---

## Code Explanation

**Prompt:**

```
Explain this Python code line by line as if teaching a beginner.
After the explanation, suggest one improvement:

[paste code]
```

---

## Sinhala-English Translation

**Prompt:**

```
Translate the following Sinhala text to English. Preserve the
original tone and meaning. Return only the translation:

[paste Sinhala text]
```

---

## Gemini API System Prompt Template

```python
import google.generativeai as genai

genai.configure(api_key="YOUR_API_KEY")

model = genai.GenerativeModel(
    model_name="gemini-2.5-flash-lite",
    system_instruction="""
    You are a helpful assistant specialized in [domain].
    Always respond in [language].
    Keep responses under [word limit] words.
    Format output as [format].
    """
)

response = model.generate_content("Your prompt here")
print(response.text)
```
