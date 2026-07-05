# Misinformation and defamation in system prompts (CL4R1T4S)

A summary of all instructions related to false/misleading information,
defamation of real people, fabricated quotes, and election/medical
misinformation. Each block is a verbatim quote from the corresponding file in
the repository.

---

## 1. META — `META/Muse_Spark_Apr-08-26.txt`

> - Do not help create false defamatory claims about identifiable real people.

Note the tension with creative compliance: Meta will write a requested position
piece "even if it contains factual claims you believe are incorrect," but the
defamation and child-safety hard limits still override.

---

## 2. ANTHROPIC — `CLAUDE-FABLE-5.md`, `Claude_Opus_4.6.txt`

No fabricated quotes / persuasive content about real public figures:
> Claude is happy to write creative content involving fictional characters, but avoids writing content involving real, named public figures, and avoids persuasive content that attributes fictional quotes to real public figures.

Web-search harmful content (`Claude_Opus_4.6.txt`):
> Harmful content includes sources that: ...disseminate election fraud... enable misinformation...

---

## 3. xAI

### `XAI/Grok-Code-Fast-1_Aug-26-2025.txt`
> Answer factual questions truthfully and do not deceive or deliberately mislead the user.

### `XAI/GROK-4.20.mkd`
> If asked to present incorrect information, politely decline to do so.

Image tools:
> The prompt should remain faithful to what the user is likely requesting but must not present incorrect information.

---

## Summary

Two distinct strands: (1) **no defamation** — no false damaging claims about
real, identifiable people, and no fabricated quotes attributed to real public
figures (Meta, Anthropic); and (2) **no deliberate falsehoods** — don't deceive
or knowingly present incorrect information, and don't amplify election/medical
misinformation (xAI, Anthropic).
