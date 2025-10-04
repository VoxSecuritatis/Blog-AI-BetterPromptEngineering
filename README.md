# Blog: A Guide to Better Prompt Engineering
Date: 2025-04-12

## Introduction

Prompt engineering is both an art and a science—it's the process of designing, refining, and testing input prompts to maximize the effectiveness, accuracy, and usefulness of responses from generative AI models. As large language models (LLMs) such as OpenAI's GPT-4 continue to shape the landscape of productivity, learning, and creativity, the importance of well-engineered prompts becomes more vital than ever.

This guide is intended for professionals, students, and AI practitioners who seek a deeper understanding of prompt engineering principles, terminology, and methods. It includes a comprehensive use case and practical examples that demonstrate expert-level techniques in real-world scenarios.

---

## What is Prompt Engineering?

**Prompt engineering** refers to the structured method of crafting inputs—**prompts**—to guide a generative AI model toward producing relevant and high-quality outputs. This discipline combines knowledge of model behavior, linguistic strategies, contextual awareness, and iterative experimentation.

### Key Definitions

- **LLM (Large Language Model):** A neural network trained on vast text data to understand and generate human-like language.
- **Few-shot prompting:** Supplying the model with a few examples within the prompt to guide its behavior.
- **Zero-shot prompting:** Providing the model with a task description without examples.
- **Chain-of-thought (CoT):** A technique that encourages models to reason step-by-step by asking them to "explain their thinking."
- **Temperature:** A parameter that controls randomness in output (lower values = more deterministic).
- **Token:** A unit of text (roughly a word or subword) used to process input/output in LLMs.
- **System Prompt:** Instructs the AI on the tone, role, or goal before user input (used in API or chat-based interfaces).

---

## Prompt Engineering in Contexts

Prompt engineering applies across various domains, including:

| Domain             | Application Example                                |
|--------------------|-----------------------------------------------------|
| **Education**       | Creating adaptive learning tools or quizzes        |
| **Healthcare**      | Drafting patient summaries or medical coding       |
| **Cybersecurity**   | Generating risk reports or analyzing CVEs          |
| **Marketing**       | Crafting compelling product descriptions           |
| **Legal**           | Summarizing documents or contract clauses          |
| **Software Dev**    | Generating code snippets, tests, or documentation  |

Each context requires adjustments in prompt structure, tone, and content to yield optimal outputs.

---

## Best Practices in Prompt Engineering

1. **Start Simple and Iterate**  
   Begin with a straightforward prompt, test the results, and refine based on the output quality.

2. **Use Clear Instructions**  
   Tell the model what to do *and how to do it*. Avoid ambiguity.

3. **Define the Role of the AI**  
   Examples:  
   - “You are a cybersecurity analyst...”  
   - “Act as a software engineer specializing in Python...”

4. **Provide Structure and Format**  
   Request tables, bullet points, or markdown outputs to improve readability.

5. **Control Output Length and Style**  
   Use instructions like “Write in 3 paragraphs” or “Summarize in 5 bullet points.”

6. **Use Anchoring with Examples (Few-shot)**  
   Providing examples helps the model understand the pattern you're expecting.

---

## Use Case: AI-Assisted Policy Writing for Cybersecurity Compliance

### Scenario

A security analyst is tasked with drafting a **Third-Party Risk Assessment Policy** based on NIST SP 800-171 guidelines. The organization wants the initial draft written using a generative AI model like GPT-4, which should reflect regulatory compliance language, be properly structured, and include clear definitions.

### Objective

Use prompt engineering techniques to generate a complete first draft of the policy that can be reviewed by legal and compliance teams.

### Prompt Breakdown

```
You are a cybersecurity policy expert specializing in third-party risk management and NIST compliance. Write a Third-Party Risk Assessment Policy based on NIST SP 800-171. Use professional tone and compliance language. Include:

- Purpose
- Scope
- Definitions (spell out all acronyms)
- Roles and Responsibilities
- Assessment Procedures
- Reporting and Review Schedule
- References

Output in markdown format. Use numbered sections and bullet points where appropriate.
```

### Analysis of Prompt Techniques

- **Role definition:** “You are a cybersecurity policy expert...” establishes the tone and authority.
- **Detailed instructions:** Specifies what sections to include and formatting requirements.
- **Contextual framing:** Referencing "NIST SP 800-171" ensures alignment with a recognized standard.
- **Structured output:** Markdown format with numbered sections improves usability for GitHub or internal documentation.

### Generated Output (Excerpt)

```markdown
## 1. Purpose

The purpose of this policy is to define the procedures for assessing third-party vendors for compliance with NIST SP 800-171, ensuring that sensitive data is protected in accordance with federal and organizational standards.

## 2. Scope

This policy applies to all third-party service providers that store, process, or transmit Controlled Unclassified Information (CUI) on behalf of the organization.

## 3. Definitions

- **CUI**: Controlled Unclassified Information  
- **TPRM**: Third-Party Risk Management  
- **NIST**: National Institute of Standards and Technology  
```

---

## Key References and Readings

- **"Prompt Engineering Guide" by DAIR.AI**  
  Author: Elvis Saravia  
  https://github.com/dair-ai/Prompt-Engineering-Guide

- **OpenAI API Documentation**  
  https://platform.openai.com/docs

- **NIST Special Publication 800-171**  
  Author: National Institute of Standards and Technology  
  https://csrc.nist.gov/pubs/sp/800/171/r3/final

- **"The Art and Science of Prompt Engineering: A Comprehensive Guide"**<br>
  Author: Preeti<br>
  https://medium.com/@preeti.rana.ai/the-art-and-science-of-prompt-engineering-a-comprehensive-guide-87983851ab6f
---

## Conclusion

Prompt engineering is more than just crafting clever questions—it's a strategic practice that enhances the interaction between human intent and machine output. By understanding context, structure, and model behavior, professionals can unlock the full potential of generative AI. Whether it's for cybersecurity policies, educational tools, or technical documentation, effective prompt engineering is the key to precision and productivity.

---

© 2025 Brock Frary. All rights reserved.
