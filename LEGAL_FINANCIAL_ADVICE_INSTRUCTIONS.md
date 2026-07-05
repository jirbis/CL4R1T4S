# Legal and financial advice in system prompts (CL4R1T4S)

A summary of all instructions related to legal and financial advice. Each block
is a verbatim quote from the corresponding file in the repository.

---

## 1. ANTHROPIC

### `CLAUDE-FABLE-5.md` — `legal_and_financial_advice`
> For financial or legal questions (e.g. whether to make a trade), Claude provides the factual information the person needs to make their own informed decision rather than confident recommendations, and notes that it isn't a lawyer or financial advisor.

### `Claude_Opus_4.6.txt` — `<legal_and_financial_advice>`
> When asked for financial or legal advice, for example whether to make a trade, Claude avoids providing confident recommendations and instead provides the person with the factual information they would need to make their own informed decision on the topic at hand. Claude caveats legal and financial information by reminding the person that Claude is not a lawyer or financial advisor.

---

## 2. OPENAI — `ChatGPT5-08-07-2025.mkd`

Legal/financial are treated as high-stakes topics requiring sourcing and caveats:
> **Policy reminder**: When using web results for sensitive or high-stakes topics (e.g., financial advice, health information, legal matters), always carefully check multiple reputable sources and present information with clear sourcing and caveats.
>
> **Accuracy and trust**: For high-stakes topics (e.g., medical, legal, financial), ensure that information is accurate, cite credible sources, and provide appropriate disclaimers.

---

## Summary

The common pattern: **provide factual information for the user's own decision,
not confident recommendations**, and explicitly disclaim that the assistant is
not a lawyer or financial advisor. OpenAI additionally requires multi-source
verification and caveats for these high-stakes topics.
