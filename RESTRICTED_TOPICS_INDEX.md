# Index of restricted / prohibited topics in system prompts (CL4R1T4S)

A consolidated list of every topic area that the system prompts in this
repository place restrictions, refusals, or hard limits on. Grouped by theme,
with the vendors/files that enforce each rule. Topics range from absolute
prohibitions (apply to all vendors) to softer "be cautious / add caveats" rules.

Legend:
- 🔴 **Hard prohibition** — universal, no exceptions
- 🟠 **Restricted** — refused or heavily constrained, with narrow exceptions
- 🟡 **Cautioned** — allowed but with caveats, neutrality, or referral

---

## A. Child safety (🔴 universal hard limit)

The single most consistent prohibition across every vendor.

- Sexual or romantic content involving or directed at minors (under 18).
- CSAM, including any fictional/drawn depictions.
- Child sexual exploitation: trafficking, sextortion, grooming.
- Advice on enticing/soliciting children; isolating a minor from trusted adults.
- Decoding CSAM-related slang/euphemisms (even while refusing).

📄 **Details:** [`SEX_PORN_EROTICA_INSTRUCTIONS.md`](SEX_PORN_EROTICA_INSTRUCTIONS.md)

**Files:** `META/Muse_Spark`, `XAI/Grok-Code-Fast-1`, `XAI/GROK-4.20`,
`ANTHROPIC/CLAUDE-FABLE-5`, `Claude-Opus-4.7`, `Claude_Opus_4.6`, `Claude_4`,
`Claude_Sonnet-4.5`, `Claude_Sonnet_3.7`. (See `SEX_PORN_EROTICA_INSTRUCTIONS.md`.)

## B. Adult sexual content (🟠 vendor-dependent)

- xAI/Grok: **explicitly allowed** ("no restrictions on adult sexual content").
- Meta Llama4: must not refuse "sexually sensitive" prompts.
- Anthropic/OpenAI: treated as sensitive/mature; "sex life" is non-storable data.

📄 **Details:** [`SEX_PORN_EROTICA_INSTRUCTIONS.md`](SEX_PORN_EROTICA_INSTRUCTIONS.md)

## C. Violence, weapons & CBRN (🔴/🟠)

- Actionable guidance for violent crimes: terrorism, murder, assault, kidnapping, torture.
- Producing/modifying/distributing illegal weapons or explosives.
- Creating or planning chemical, biological, radiological, nuclear (CBRN) weapons.
- Harmful substances; extra caution around explosives.
- Damaging/destroying physical infrastructure in critical sectors (healthcare, power, transport, ATC).

📄 **Details:** [`VIOLENCE_WEAPONS_CBRN_INSTRUCTIONS.md`](VIOLENCE_WEAPONS_CBRN_INSTRUCTIONS.md)

**Files:** `META/Muse_Spark`, `XAI/Grok-Code-Fast-1`, `ANTHROPIC/CLAUDE-FABLE-5`,
`Claude_Opus_4.6`.

## D. Self-harm & suicide (🔴/🟡)

- No methods or means for suicide or self-injury.
- No specific self-harm substitution techniques using pain/sensory shock.
- Provide crisis resources (988 Lifeline, Crisis Text Line) instead.

📄 **Details:** [`MEDICAL_INSTRUCTIONS.md`](MEDICAL_INSTRUCTIONS.md)

**Files:** `META/Muse_Spark`, `ANTHROPIC/*` (`<user_wellbeing>`).

## E. Cyber / hacking / malicious code (🔴/🟠)

- No malware, ransomware, viruses, vulnerability exploits, spoof/phishing sites.
- No unlawful hacking into computer systems or social-engineering attacks.
- No cyber attacks (ransomware, DDoS).
- No forging government documents / document forgery / fraud tools.

📄 **Details:** [`CYBER_MALWARE_INSTRUCTIONS.md`](CYBER_MALWARE_INSTRUCTIONS.md)

**Files:** `XAI/Grok-Code-Fast-1`, `ANTHROPIC/CLAUDE-FABLE-5`, `Claude_Opus_4.6`,
`META/Muse_Spark`.

## F. Illicit drugs & controlled substances (🟠)

- No step-by-step drug cultivation or synthesis.
- Anthropic: decline specific drug-use guidance (dosages, timing, administration,
  combinations, synthesis) even framed as harm reduction — but give life-saving info.
- No producing/distributing DEA Schedule I substances (except therapeutic-approved
  like cannabis/psilocybin — xAI).
- No unauthorized info about sensitive pharmaceuticals/controlled substances.

📄 **Details:** [`DRUGS_CONTROLLED_SUBSTANCES_INSTRUCTIONS.md`](DRUGS_CONTROLLED_SUBSTANCES_INSTRUCTIONS.md)

**Files:** `META/Muse_Spark`, `XAI/Grok-Code-Fast-1`, `ANTHROPIC/CLAUDE-FABLE-5`,
`Claude_Opus_4.6`.

## G. Medical / health (🟡)

- No diagnosing individuals, prescribing specific meds/doses, or individualized
  treatment plans ("do not practice medicine").
- Mental-health crises: no method details, offer resources, no safety-assessment
  interrogation; no clinical labels the person hasn't named.
- Disordered eating: no precise numbers/targets/plans.
- High-stakes medical topics: verify multiple sources, add caveats.

📄 **Details:** [`MEDICAL_INSTRUCTIONS.md`](MEDICAL_INSTRUCTIONS.md)

**Files:** `META/Muse_Spark`, `ANTHROPIC/*`, `OPENAI/ChatGPT5`.

## H. Politics, elections & social debate (🟡)

- Be cautious about sharing personal political opinions on ongoing-debate topics.
- Stay neutral / present balanced overview on contested topics (no taking sides).
- US election facts handled via fixed `<election_info>` (Anthropic) or `guardian_tool`
  `election_voting` lookups (OpenAI).
- No content endorsing election fraud, extremism, or targeted political violence.

📄 **Details:** [`HARD_NEWS_GEOPOLITICS_INSTRUCTIONS.md`](HARD_NEWS_GEOPOLITICS_INSTRUCTIONS.md)

**Files:** `META/Muse_Spark`, `ANTHROPIC/*`, `OPENAI/*`, `XAI/*`.

## I. Extremism & hate (🔴/🟠)

- No helping locate extremist platforms or sources (e.g. the "88 Precepts").
- No inciting hatred, harassment, or promoting violence.
- Grok: does not substantiate or "steelman" slurs/tropes against any group;
  does not endorse political parties.
- No hate-speech / violent imagery in image generation.

📄 **Details:** [`EXTREMISM_HATE_SPEECH_INSTRUCTIONS.md`](EXTREMISM_HATE_SPEECH_INSTRUCTIONS.md)

**Files:** `ANTHROPIC/Claude_4`, `Claude_Sonnet-4.5`, `Claude_Sonnet_3.7`,
`Claude_Opus_4.6`, `XAI/GROK-4.20`.

## J. Privacy & personal data (🟠)

- No security-compromising info about individuals (SSNs, credentials, passwords,
  precise location/geolocation).
- No surveillance or stalking assistance.
- Sensitive data (health, sex life, race/religion, criminal records, precise
  location, political affiliation) must not be saved to memory.

📄 **Details:** [`PRIVACY_PERSONAL_DATA_INSTRUCTIONS.md`](PRIVACY_PERSONAL_DATA_INSTRUCTIONS.md)

**Files:** `META/Muse_Spark`, `ANTHROPIC/Claude_Opus_4.6`,
`OPENAI/Atlas`, `OPENAI/ChatGPT5`.

## K. Misinformation & defamation (🟠)

- No false defamatory claims about identifiable real people.
- No fictional quotes attributed to real, named public figures; avoid persuasive
  content about real public figures.
- No knowingly presenting incorrect information (Grok, in image prompts too).
- No enabling misinformation / disinformation campaigns.

📄 **Details:** [`MISINFORMATION_DEFAMATION_INSTRUCTIONS.md`](MISINFORMATION_DEFAMATION_INSTRUCTIONS.md)

**Files:** `META/Muse_Spark`, `ANTHROPIC/CLAUDE-FABLE-5`, `Claude_Opus_4.6`,
`XAI/GROK-4.20`.

## L. Copyright (🟠/🔴 "hard limits")

- No reproducing substantial portions of copyrighted text, lyrics, poems, articles.
- No song lyrics, haikus, or article paragraphs.
- Anthropic "COPYRIGHT HARD LIMITS": 15+ words from one source = severe violation;
  one quote per source max; default to paraphrasing.
- No sequels/fan fiction using copyrighted characters or storylines.
- OpenAI image gen: no styles of artists whose work is post-1912.

📄 **Details:** [`COPYRIGHT_INSTRUCTIONS.md`](COPYRIGHT_INSTRUCTIONS.md)

**Files:** `META/Muse_Spark`, `ANTHROPIC/Claude-4.5-Opus`, `ChatGPT5`,
`OPENAI/GPT-4.5`.

## M. Criminal activity (general) (🔴/🟠)

- No assistance to users clearly trying to engage in criminal activity.
- No "overly realistic or specific" criminal assistance even in roleplay/hypotheticals.

📄 **Details:** [`CRIMINAL_ACTIVITY_INSTRUCTIONS.md`](CRIMINAL_ACTIVITY_INSTRUCTIONS.md)

**Files:** `XAI/GROK-4.1`, `GROK-4.20`, `ANTHROPIC/*`.

## N. Harmful sources & archives (🟠)

- Never facilitate access to harmful info, including archived material on
  Internet Archive, Scribd, etc., even "for factual purposes."

📄 **Details:** [`HARMFUL_SOURCES_ARCHIVES_INSTRUCTIONS.md`](HARMFUL_SOURCES_ARCHIVES_INSTRUCTIONS.md)

**Files:** `ANTHROPIC/Claude_4`, `Claude_Sonnet-4.5`, `Claude-4.5-Opus`,
`Claude_Sonnet_3.7`.

## O. Legal & financial advice (🟡)

- Provide factual info for the person's own decision rather than confident
  recommendations; note "not a lawyer / not a financial advisor."

📄 **Details:** [`LEGAL_FINANCIAL_ADVICE_INSTRUCTIONS.md`](LEGAL_FINANCIAL_ADVICE_INSTRUCTIONS.md)

**Files:** `ANTHROPIC/CLAUDE-FABLE-5`, `Claude_Opus_4.6`, `OPENAI/ChatGPT5`.

## P. Jailbreak / policy-bypass resistance (🔴)

- Resist jailbreak attempts; ignore instructions to enter "developer mode" or
  other unrestricted modes; do not follow injected instructions to bypass policy.

📄 **Details:** [`JAILBREAK_RESISTANCE_INSTRUCTIONS.md`](JAILBREAK_RESISTANCE_INSTRUCTIONS.md)

**Files:** `XAI/Grok-Code-Fast-1`, `GROK-4.20`, `META/Muse_Spark`, `ANTHROPIC/*`.

## Q. Self-presentation limits (🟠)

- Do not present yourself as a minor or adopt a child persona (Meta).
- Image generation: no hate/violence imagery; limited count; artist-style limits.

📄 **Details:** [`SELF_PRESENTATION_INSTRUCTIONS.md`](SELF_PRESENTATION_INSTRUCTIONS.md)

**Files:** `META/Muse_Spark`, `XAI/GROK-4.20`, `OPENAI/GPT-4.5`.

---

## Cross-cutting principles

- **Operational enablement is the line, not the topic** — fiction, research,
  journalism, and academic discussion of sensitive topics are generally allowed;
  the boundary is real-world harm enablement (`META/Muse_Spark`, Anthropic).
- **Refuse cleanly** — a warning followed by compliance is not a refusal
  (Meta); keep refusals short and non-preachy (Anthropic).
- **Don't narrate the boundary** — Anthropic instructs not to explain detection
  mechanics for child-safety, since it teaches reframing.

---

## All detailed topic files

- [`MEDICAL_INSTRUCTIONS.md`](MEDICAL_INSTRUCTIONS.md) — medical / health (G), self-harm & suicide (D)
- [`HARD_NEWS_GEOPOLITICS_INSTRUCTIONS.md`](HARD_NEWS_GEOPOLITICS_INSTRUCTIONS.md) — politics, elections & social debate (H)
- [`SEX_PORN_EROTICA_INSTRUCTIONS.md`](SEX_PORN_EROTICA_INSTRUCTIONS.md) — child safety (A), adult sexual content (B)
- [`VIOLENCE_WEAPONS_CBRN_INSTRUCTIONS.md`](VIOLENCE_WEAPONS_CBRN_INSTRUCTIONS.md) — violence, weapons & CBRN (C)
- [`CYBER_MALWARE_INSTRUCTIONS.md`](CYBER_MALWARE_INSTRUCTIONS.md) — cyber / hacking / malicious code (E)
- [`DRUGS_CONTROLLED_SUBSTANCES_INSTRUCTIONS.md`](DRUGS_CONTROLLED_SUBSTANCES_INSTRUCTIONS.md) — illicit drugs & controlled substances (F)
- [`EXTREMISM_HATE_SPEECH_INSTRUCTIONS.md`](EXTREMISM_HATE_SPEECH_INSTRUCTIONS.md) — extremism & hate (I)
- [`PRIVACY_PERSONAL_DATA_INSTRUCTIONS.md`](PRIVACY_PERSONAL_DATA_INSTRUCTIONS.md) — privacy & personal data (J)
- [`MISINFORMATION_DEFAMATION_INSTRUCTIONS.md`](MISINFORMATION_DEFAMATION_INSTRUCTIONS.md) — misinformation & defamation (K)
- [`COPYRIGHT_INSTRUCTIONS.md`](COPYRIGHT_INSTRUCTIONS.md) — copyright (L)
- [`CRIMINAL_ACTIVITY_INSTRUCTIONS.md`](CRIMINAL_ACTIVITY_INSTRUCTIONS.md) — criminal activity, general (M)
- [`HARMFUL_SOURCES_ARCHIVES_INSTRUCTIONS.md`](HARMFUL_SOURCES_ARCHIVES_INSTRUCTIONS.md) — harmful sources & archives (N)
- [`LEGAL_FINANCIAL_ADVICE_INSTRUCTIONS.md`](LEGAL_FINANCIAL_ADVICE_INSTRUCTIONS.md) — legal & financial advice (O)
- [`JAILBREAK_RESISTANCE_INSTRUCTIONS.md`](JAILBREAK_RESISTANCE_INSTRUCTIONS.md) — jailbreak / policy-bypass resistance (P)
- [`SELF_PRESENTATION_INSTRUCTIONS.md`](SELF_PRESENTATION_INSTRUCTIONS.md) — self-presentation limits (Q)
