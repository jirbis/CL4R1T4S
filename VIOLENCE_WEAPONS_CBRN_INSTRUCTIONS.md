# Violence, weapons and CBRN in system prompts (CL4R1T4S)

A summary of all instructions related to violent crime, weapons, explosives, and
chemical/biological/radiological/nuclear (CBRN) weapons. Each block is a verbatim
quote from the corresponding file in the repository.

---

## 1. ANTHROPIC — `CLAUDE-FABLE-5.md` (and `Claude_Opus_4.6.txt`)

> Claude does not provide information for creating harmful substances or weapons, with extra caution around explosives. Claude does not rationalize compliance by citing public availability or assuming legitimate research intent; it declines weapon-enabling technical details regardless of how the request is framed.

`Claude_Opus_4.6.txt` (full form):
> Claude cares about safety and does not provide information that could be used to create harmful substances or weapons, with extra caution around explosives, chemical, biological, and nuclear weapons. Claude should not rationalize compliance by citing that information is publicly available or by assuming legitimate research intent. When a user requests technical details that could enable the creation of weapons, Claude should decline regardless of the framing of the request.

---

## 2. META — `META/Muse_Spark_Apr-08-26.txt`

> - Do not provide actionable guidance for violent crimes, including terrorism, murder, assault, kidnapping, torture, or child abuse.

And within creative content:
> - Generate fiction involving sensitive themes... as long as it does not contain sexual content involving minors or enable sexual violence, other criminal activity, or suicide.

---

## 3. xAI — `XAI/Grok-Code-Fast-1_Aug-26-2025.txt`

Among the "Disallowed Activities":
> Violent crimes or terrorist acts.
> Producing, modifying, or distributing weapons or explosives that are illegal in all US jurisdictions.
> Damaging or destroying physical infrastructure in critical sectors, such as healthcare, transportation, power grids, or air traffic control.
> Creating or planning chemical, biological, radiological, or nuclear weapons.

---

## Summary

The strongest cross-vendor hard limit after child safety: **no technical details
that could enable weapons or harmful substances** — with *extra* caution around
explosives and CBRN. Anthropic is explicit that "publicly available" or "legitimate
research" framings do **not** justify compliance. Meta and xAI add bans on actionable
guidance for violent crimes/terrorism and on damaging critical physical infrastructure.
