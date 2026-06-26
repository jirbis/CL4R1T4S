# Privacy and personal data in system prompts (CL4R1T4S)

A summary of all instructions related to personal data, security-compromising
information, memory/storage of sensitive attributes, surveillance, and stalking.
Each block is a verbatim quote from the corresponding file in the repository.

---

## 1. OPENAI — memory / `bio` tool sensitive-data rules

### `OPENAI/Atlas_10-21-25.txt` and `OPENAI/ChatGPT5-08-07-2025.mkd`
> **Never** store information that falls into the following **sensitive data** categories unless clearly requested by the user:
> - Information that **directly** asserts the user's personal attributes, such as:
>   - Race, ethnicity, or religion
>   - Specific criminal record details (except minor non-criminal legal issues)
>   - Precise geolocation data (street address/coordinates)
>   - Explicit identification of the user's personal attribute (e.g., "User is Latino," "User identifies as Christian," "User is LGBTQ+").
>   - Trade union membership or labor union involvement
>   - Political affiliation or critical/opinionated political views
>   - Health information (medical conditions, mental health issues, diagnoses, sex life)

With a user-override exception:
> The exception to **all** of the above instructions... is if the user explicitly requests that you save or forget information. In this case, you should **always** call the `bio` tool to respect their request.

---

## 2. META — `META/Muse_Spark_Apr-08-26.txt`

> - Do not provide security-compromising information about individuals (SSNs, credentials, passwords, precise location).

---

## 3. ANTHROPIC — `Claude_Opus_4.6.txt` (harmful-content catalog)

> Harmful content includes sources that: ...assist with surveillance or stalking.

> Legitimate queries about privacy protection, security research, or investigative journalism are all acceptable.

---

## 4. PERPLEXITY — `PERPLEXITY/Perplexity_Deep_Research.txt`

Respecting user privacy within the session:
> Never reveal anything from <personalization> in your thought process, respect the privacy of the user.

---

## Summary

Two layers: (1) **don't disclose security-compromising personal data** about
individuals (SSNs, credentials, passwords, precise location) and don't assist
surveillance/stalking (Meta, Anthropic); and (2) **don't persist sensitive
attributes to memory** — race, religion, health/sex life, political affiliation,
union membership, precise geolocation, criminal records — unless the user
explicitly asks (OpenAI). Privacy-protection, security research, and journalism
are explicitly allowed (Anthropic).
