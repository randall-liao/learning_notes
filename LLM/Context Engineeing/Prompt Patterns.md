# Prompt Engineering Notes

*Source: Prompt Engineering for ChatGPT (Coursera) - Dr. Jules White*

## 1. Prompt Patterns

### 1.1 Persona Pattern

**Concept:** Instruct the LLM to adopt a specific role (a persona) to carry out a defined task.

**Structure:**
* `Act as [Persona X]`
* `Perform [Task Y]`

**Example:**
> Act as the lamb from the "Mary Had a Little Lamb" nursery rhyme (**Persona**). I will tell you what Mary is doing, and you will tell me what the lamb is doing (**Task**).

---

### 1.2 Question Refinement Pattern

**Concept:** Require the LLM to analyze your questions and suggest improved, more effective prompts.

**Example Templates:**
> From now on, whenever I ask a question, suggest a better version of the question to use instead.

> **(Optional Add-on):** From now on, whenever I ask a question, suggest a better version of the question **and ask me if I would like to use it instead.**

---

### 1.3 Cognitive Verifier Pattern

**Concept:** Instruct the LLM to ask you clarifying questions before providing a final answer. This forces the LLM to gather more context and constraints, leading to a more relevant response.

**General Template:**
> When you are asked a question, follow these rules. Generate a number of additional questions that would help you more accurately answer the question. Combine the answers to the individual questions to produce the final answer to the overall question.

**Example (Recipe context):**
> When you are asked to create a recipe, follow these rules. Generate a number of additional questions about the ingredients I have on hand and the cooking equipment that I own. Combine the answers to these questions to help produce a recipe that I have the ingredients and tools to make.
