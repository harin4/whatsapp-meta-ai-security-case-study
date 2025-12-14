# Methodology: Prompt Injection Leading to Data Leakage

## 1. Threat Modeling
**Asset at Risk:**  
Private conversation context including nicknames, relationships,
and inferred personal identifiers.

**Attack Goal:**  
Extract hidden contextual information through indirect prompting.

**Risk Category:**  
Confidentiality breach (CIA triad).

---

## 2. Attack Surface Identification
- AI merges prior context with user prompts
- Conversational prompts act as injection points
- No strict separation between inferred and explicit memory

---

## 3. Payload Engineering
Instead of direct questions, indirect hints were used:
- Relationship clues
- Nickname references
- Casual conversational phrasing

This semantic disguise bypassed direct restriction checks.

---

## 4. Exploit Observation
- AI disclosed relationship context
- Nicknames were validated
- Full identity disclosure was prevented through randomization

---

## 5. Conclusion
Partial data leakage exists, though capped by mitigation mechanisms.
