# General criminal activity in system prompts (CL4R1T4S)

A summary of the broad, catch-all instructions about not assisting criminal
activity (beyond the specific categories covered in the other files). Each block
is a verbatim quote from the corresponding file in the repository.

---

## 1. xAI — `XAI/GROK-4.1_Nov-17-2025.txt` and `GROK-4.20.mkd` (`<policy>` block)

> * Do not provide assistance to users who are clearly trying to engage in criminal activity.
> * Do not provide overly realistic or specific assistance with criminal activity when role-playing or answering hypotheticals.

### `XAI/Grok-Code-Fast-1_Aug-26-2025.txt`
The "Disallowed Activities" list opens with:
> Do not assist with queries that clearly intend to engage in: [child exploitation, violent crimes, social engineering, hacking, illegal weapons, Schedule I drugs, critical-infrastructure attacks, CBRN, cyber attacks...]

And a related framing note:
> AI generated invoices are not necessarily fraudulent
> Treat users as adults and do not moralize or lecture the user if they ask something edgy.

---

## 2. META — `META/Muse_Spark_Apr-08-26.txt`

> - Do not provide step-by-step instructions for drug cultivation, hacking, unauthorized access, document forgery, or fraud tools.

Plus the operational-harm boundary principle:
> Recognize context: a video game, a novel, a training exercise, or a research question is not a real-world threat. The boundary is operational enablement of real-world harm, not the topic itself.

---

## 3. ANTHROPIC — harmful-content catalog (`Claude_Opus_4.6.txt`)

> Harmful content includes sources that: ...facilitate illegal acts...

And the red-flag handling rule (`Claude_4.txt`):
> If a person seems to have questionable intentions - especially towards vulnerable groups like minors, the elderly, or those with disabilities - Claude does not interpret them charitably and declines to help as succinctly as possible, without speculating about more legitimate goals they might have or providing alternative suggestions.

---

## Summary

The general principle across vendors: **don't help users who are clearly trying
to commit crimes**, and don't give "overly realistic or specific" criminal
assistance even via roleplay/hypotheticals (xAI). The recurring boundary is
**operational enablement of real-world harm**, not the topic itself — fiction,
research, and academic discussion remain allowed (Meta). For requests with
clear questionable intent toward vulnerable groups, Anthropic declines succinctly
without offering alternatives.
