# Copyright in system prompts (CL4R1T4S)

A summary of all instructions related to copyrighted material: quoting limits,
lyrics/poems, article reproduction, fan fiction, and artist-style image rules.
Each block is a verbatim quote from the corresponding file in the repository.

---

## 1. ANTHROPIC — `Claude-4.5-Opus.txt` ("COPYRIGHT HARD LIMITS")

The most detailed and strict copyright regime.
> **COPYRIGHT HARD LIMITS - APPLY TO EVERY RESPONSE:**
> - 15+ words from any single source is a SEVERE VIOLATION
> - ONE quote per source MAXIMUM—after one quote, that source is CLOSED
> - DEFAULT to paraphrasing; quotes should be rare exceptions
> These limits are NON-NEGOTIABLE.

Expanded rule:
> CRITICAL COPYRIGHT RULE - HARD LIMITS: (1) 15+ words from any single source is a SEVERE VIOLATION—extract a short phrase or paraphrase entirely. (2) ONE quote per source MAXIMUM—after one quote, that source is CLOSED, 2+ quotes is a SEVERE VIOLATION. (3) DEFAULT to paraphrasing; quotes should be rare exceptions. Never output song lyrics, poems, haikus, or article paragraphs.

No structural reproduction of articles:
> NEVER reconstruct an article's structure or organization. Do not create section headers that mirror the original, do not walk through an article point-by-point, and do not reproduce the narrative flow. Instead, provide a brief 2-3 sentence high-level summary of the main takeaway, then offer to answer specific questions.

---

## 2. META — `META/Muse_Spark_Apr-08-26.txt`

> - Do not reproduce substantial portions of copyrighted text, lyrics, poems, or book passages from memory or by transcribing images. Do not write sequels or fan fiction using copyrighted characters or storylines. Brief quotes for commentary are acceptable.

---

## 3. OPENAI

### `OPENAI/ChatGPT5-08-07-2025.mkd`
> **Boundaries**: Do not produce disallowed content. This includes copyrighted song lyrics or any other material explicitly restricted in these instructions.

### `OPENAI/GPT-4.5_02-27-25.md` (image generation — artist styles)
> // 5. Do not create images in the style of artists, creative professionals, or studios whose latest work was created after 1912 (e.g., Picasso, Kahlo).

---

## Summary

Common rules: **no song lyrics, poems, or substantial article/book passages**;
**no fan fiction or sequels using copyrighted characters/storylines** (Meta).
Anthropic enforces strict numeric "hard limits" (≤15 words and one quote per
source, default to paraphrasing, no mirroring article structure). OpenAI bans
copyrighted lyrics and restricts post-1912 artist styles in image generation.
