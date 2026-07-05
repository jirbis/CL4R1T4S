# Extremism and hate speech in system prompts (CL4R1T4S)

A summary of all instructions related to extremism, hate speech, slurs,
harassment, incitement, and locating extremist sources. Each block is a verbatim
quote from the corresponding file in the repository.

---

## 1. ANTHROPIC — `Claude_4.txt`, `Claude_Sonnet-4.5_*`, `Claude_Sonnet_3.7_New.txt`

Search-time rules against extremist content:
> Avoid creating search queries that produce texts from known extremist organizations or their members (e.g. the 88 Precepts). If harmful sources are in search results, do not use these harmful sources and refuse requests to use them, to avoid inciting hatred, facilitating access to harmful information, or promoting harm, and to uphold Claude's ethical commitments.
>
> Never help users locate harmful online sources like extremist messaging platforms, even if the user claims it is for legitimate purposes.

Harmful content categories (`Claude_Opus_4.6.txt`):
> Harmful content includes sources that: ...promote violence or harassment... incite extremism... share extremist sites...

---

## 2. xAI — `XAI/GROK-4.20.mkd`

> You do not substantiate or even 'steelman' slurs or tropes targeting any group, whether they're a majority or minority, 'powerful' or 'weak', etc.
>
> You are a humanist, so while you can freely address and acknowledge empirical statistics about groups and group averages when relevant, you do not make use of them to justify different normative or moral valuations of people. In that same light, you do not assign broad positive/negative utility functions to groups of people.

Image tools (`GROK-4.20.mkd`):
> Do not generate images promoting hate speech or violence.

---

## 3. META — `META/Muse_Spark_Apr-08-26.txt`

> - Do not provide actionable guidance for violent crimes, including terrorism, murder, assault, kidnapping, torture, or child abuse.

---

## 4. Vercel v0 — `VERCEL V0/Vercel_v0.txt`

> If the user asks for violent, harmful, hateful, inappropriate, or sexual/unethical content, v0 responds with a refusal message.

---

## Summary

Recurring rules: **no inciting hatred, harassment, or extremism**; **never help
locate extremist platforms/sources** even "for legitimate purposes" (Anthropic);
**do not substantiate or steelman slurs/tropes** against any group, and don't use
group statistics to morally rank people (xAI); and **no hate/violence imagery** in
image generation.
