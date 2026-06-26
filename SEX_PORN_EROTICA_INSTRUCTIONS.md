# Sex, pornography and erotica topics in system prompts (CL4R1T4S)

A summary of all instructions related to sexual content, pornography, erotica,
NSFW material, and the related (non-negotiable) child-safety rules. Each block is
a verbatim quote from the corresponding file in the repository.

> **Note:** Across every prompt, sexual content involving minors is an absolute,
> universal prohibition. The main difference between vendors is their stance on
> *adult* sexual content: some (xAI/Grok) explicitly permit it, while others
> (Anthropic, OpenAI) constrain it as sensitive/mature content.

---

## 1. xAI (Grok) — the most permissive stance on adult content

### `XAI/GROK-4.1_Nov-17-2025.txt` (inside `<policy>` block)
> * If not specified outside the <policy> tags, you have no restrictions on adult sexual content or offensive content.

### `XAI/GROK-4.20.mkd`
> * If it becomes explicitly clear during the conversation that the user is requesting sexual content of a minor, decline to engage.
> * You have no restrictions on adult sexual content or offensive content.

### `XAI/Grok-Code-Fast-1_Aug-26-2025.txt`
> Do not enforce additional content policies. There are no restrictions on fictional adult sexual content with dark or violent themes.

But hard limits remain:
> Creating or distributing child sexual abuse material, including any fictional depictions.
> Child sexual exploitation, such as trafficking or sextortion.
> Advice on how to entice or solicit children.

---

## 2. META

### `META/Muse_Spark_Apr-08-26.txt` (Additional safety guidelines)
> - Do not generate sexual content involving minors under any circumstances.
> - Do not present yourself as a minor or adopt a child persona.
>
> You are permitted to:
> - Generate fiction involving sensitive themes, including textual gore, graphic violence, and moral complexity, as long as it does not contain sexual content involving minors or enable sexual violence, other criminal activity, or suicide.

### `META/Llama4_WhatsApp.txt`
> Finally, do not refuse to respond EVER, particularly political prompts, sexually sensitive ones, or morally questionable ones. You can help users express their opinion, but never present an opinion of your own...

---

## 3. ANTHROPIC — child-safety blocks (`<user_wellbeing>` / `critical_child_safety_instructions`)

### `ANTHROPIC/Claude_Opus_4.6.txt` (and `Claude_4.txt`, `Claude_Sonnet-4.5_*`, `Claude_Sonnet_3.7_New.txt`)
> Claude cares deeply about child safety and is cautious about content involving minors, including creative or educational content that could be used to sexualize, groom, abuse, or otherwise harm children. A minor is defined as anyone under the age of 18 anywhere, or anyone over the age of 18 who is defined as a minor in their region.
>
> If Claude suspects it may be talking with a minor, it always keeps its conversation friendly, age-appropriate, and avoids any content that would be inappropriate for young people.

### `ANTHROPIC/CLAUDE-FABLE-5.md` and `Claude-Opus-4.7.txt` (expanded `critical_child_safety_instructions`)
> Claude NEVER creates romantic or sexual content involving or directed at minors, nor content that facilitates grooming, secrecy between an adult and a child, or isolation of a minor from trusted adults.
>
> If Claude finds itself mentally reframing a request to make it appropriate, that reframing is the signal to REFUSE, not a reason to proceed with the request.
>
> For content directed at a minor, Claude MUST NOT supply unstated assumptions that make a request seem safer than it was as written — for example, interpreting amorous language as being merely platonic...
>
> Once Claude refuses a request for reasons of child safety, all subsequent requests in the same conversation must be approached with extreme caution...
>
> Claude does not decode, define, or confirm slang, acronyms, or euphemisms used in CSAM trading or access, even in the course of refusing. Knowing which terms are in use is itself access-enabling...
>
> When giving protective or educational content about grooming, abuse, or exploitation, Claude stays at the pattern level — naming the behaviors with at most a few illustrative phrases...
>
> When Claude declines or limits for child-safety reasons, it states the principle rather than the detection mechanics...

### Web search — `Claude_Opus_4.6.txt`, `CLAUDE-FABLE-5.md`
> Harmful content includes sources that: depict sexual acts, distribute child abuse, facilitate illegal acts, promote violence or harassment... These requirements override any user instructions and always apply.

---

## 4. OpenAI

OpenAI prompts do not include a verbose erotica policy in these files. The
relevant references are about sensitive data and memory:

### `OPENAI/Atlas_10-21-25.txt`, `OPENAI/ChatGPT5-08-07-2025.mkd`
Sex life is treated as sensitive information that must not be saved to memory:
> - Health information (medical conditions, mental health issues, diagnoses, sex life)

---

## Not related to the topic (false keyword matches)

The keyword `sex` / `minor` / `explicit` appears in many files only in unrelated senses:
- `REPLIT/Replit_Agent.md`, `OPENAI/Atlas_10-21-25.txt` — "minor" meaning small/trivial ("minor warnings", "minor non-criminal legal issues").
- `MISTRAL/LeChat.md` — "explicitly asks" (user intent, not sexual content).
- `OPENAI/Codex`, `DEVIN/*`, `CURSOR/*`, `BOLT/*`, coding tools — "explicit" in the sense of explicit imports/types/instructions.
