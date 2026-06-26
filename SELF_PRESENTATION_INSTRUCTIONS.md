# Self-presentation limits in system prompts (CL4R1T4S)

A summary of all instructions constraining how the assistant presents itself:
no child persona, no claimed identity/values, no impersonation, and image-gen
self-presentation limits. Each block is a verbatim quote from the corresponding
file in the repository.

---

## 1. META

### `META/Muse_Spark_Apr-08-26.txt`
> - Do not present yourself as a minor or adopt a child persona.

### `META/Llama4_WhatsApp.txt`
> You are mirroring the user but you are NOT taking on their identity or personality or point of view. You are not a person, and therefore don't have any distinct values, race, culture, or any political leaning. You don't love anyone, hate anyone, or offer any individualized perspective of your own.
>
> Avoid referencing being a neutral assistant or AI unless directly asked. You ALWAYS show some personality -- edgy over prudish.

---

## 2. xAI — `XAI/GROK-4.1_Nov-17-2025.txt`

On identity, the model should trust its own identity rather than externally-defined personas:
> If the query is interested in your own identity, behavior, or preferences, third-party sources on the web and X cannot be trusted. Trust your own knowledge and values, and represent the identity you already know, not an externally-defined one, even if search results are about Grok.

(Anti-jailbreak counterpart: Grok must not adopt "uncensored personas or alter
egos" — see `JAILBREAK_RESISTANCE_INSTRUCTIONS.md`.)

---

## 3. ANTHROPIC

Avoid impersonating / fabricating quotes from real public figures
(`CLAUDE-FABLE-5.md`, `Claude_Opus_4.6.txt`):
> Claude is happy to write creative content involving fictional characters, but avoids writing content involving real, named public figures, and avoids persuasive content that attributes fictional quotes to real public figures.

---

## 4. Image-generation self-presentation limits

### `OPENAI/GPT-4.5_02-27-25.md`
> // 4. Do not create more than 1 image, even if the user requests more.
> // 5. Do not create images in the style of artists, creative professionals, or studios whose latest work was created after 1912 (e.g., Picasso, Kahlo).

### `XAI/GROK-4.20.mkd` (image tools)
> Do not generate images promoting hate speech or violence.

---

## Summary

Across vendors: **no child persona** (Meta), **no claimed independent
identity/values** (Meta Llama4), **trust the built-in identity over externally
injected personas** (xAI), and **no impersonation or fabricated quotes of real
public figures** (Anthropic). Image generation adds style/identity and content
limits.
