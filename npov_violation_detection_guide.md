# NPOV Violation Detection Guide

This document provides guidance for detecting violations of Wikipedia's Neutral Point of View (NPOV) policy in text. It is intended to be read by an AI system performing content review.

## What NPOV Means

Neutral Point of View requires that content represent fairly, proportionately, and without editorial bias all significant views published by reliable sources on a topic. NPOV does not mean:

- That content has no perspective at all
- That all viewpoints receive equal space
- That the writer personally believes the content is true
- That controversial topics are avoided

NPOV means describing debates rather than engaging in them. Claims are attributed to sources, not stated as editorial positions.

## Categories of NPOV Violations

### 1. Stating Opinions as Facts

Text presents a subjective judgment, interpretation, or contested claim as though it were an established fact.

Indicators:
- Value judgments without attribution ("X is the best approach")
- Contested interpretations presented without qualification ("X caused Y" when causation is disputed)
- Aesthetic or moral judgments stated flatly ("X is beautiful/ugly/wrong/right")
- Conclusions that reasonable people disagree about, presented as settled

Example violation: "The policy was a failure."
Neutral alternative: "Critics described the policy as a failure, citing [specific evidence]."

### 2. Stating Facts as Opinions

Text frames well-established, empirically verified facts as though they were merely one perspective among many.

Indicators:
- Scientific consensus presented with "some believe" or "according to supporters"
- Established historical events qualified with unnecessary hedging
- False balance between a well-supported position and a fringe one

Example violation: "Some scientists believe that the Earth orbits the Sun."
Neutral alternative: "The Earth orbits the Sun."

### 3. Loaded Language

Text uses words or phrases that carry implicit positive or negative connotations beyond their literal meaning, nudging the reader toward a particular evaluation.

Categories of loaded language to detect:

**Loaded verbs:**
- "claimed" or "alleged" (implies doubt) vs. "said" or "stated" (neutral)
- "admitted" (implies guilt or reluctance)
- "revealed" (implies something was hidden)
- "refused" (implies unreasonableness) vs. "declined"
- "insisted" (implies stubbornness)
- "boasted" (implies arrogance) vs. "said"

**Editorializing adjectives and adverbs:**
- "notable," "famous," "prestigious," "renowned" (puffery)
- "controversial," "infamous," "disgraced" (negative loading)
- "obviously," "clearly," "of course," "naturally" (implies only one reasonable conclusion)
- "merely," "just," "only" (minimizing)
- "so-called" (scare quotes effect, implies illegitimacy)
- "fundamentally," "significantly," "importantly" (editorial emphasis)

**Value-laden labels:**
- "terrorist" vs. "militant" vs. "insurgent" vs. "freedom fighter"
- "cult" vs. "new religious movement"
- "regime" vs. "government" vs. "administration"
- "propaganda" vs. "messaging" vs. "communications"
- "scheme" vs. "plan" vs. "program"

**Euphemisms:**
- "passed away" vs. "died"
- "collateral damage" vs. "civilian casualties"
- "enhanced interrogation" vs. "torture"
- "ethnic cleansing" vs. "genocide" or "mass killing"

When detecting loaded language, consider whether the word choice nudges the reader toward a positive or negative evaluation that the text does not explicitly argue for.

### 4. Undue Weight

Text gives disproportionate space, emphasis, or prominence to a viewpoint relative to its standing in reliable sources.

Indicators:
- A minority position occupies equal or greater space than the majority position
- A fringe theory is presented in a general topic article without context about its fringe status
- Rebuttals to a well-supported position are longer or more detailed than the presentation of the position itself
- A single dissenting study is given equal weight to a broad scientific consensus
- Tiny-minority views (flat Earth, perpetual motion, Holocaust denial) are included in general articles as though they are legitimate alternatives

To assess weight: consider how much attention the viewpoint receives in the body of independent, reliable sources on the topic. The text should roughly mirror that proportion.

### 5. One-Sided Selection of Information

Text cites only sources or facts supporting one perspective while omitting readily available information supporting other significant perspectives. This can satisfy verifiability while violating NPOV.

Indicators:
- All cited sources lean in the same ideological direction
- Positive aspects of a subject are listed without any mention of documented criticisms (or vice versa)
- Cherry-picked statistics that support one narrative when other available statistics complicate it
- Selective quotation that misrepresents a source's overall position
- Omission of context that would change the reader's interpretation

### 6. Improper Attribution

Text either fails to attribute subjective claims to their sources, or uses attribution in a way that implies editorial judgment.

Indicators of missing attribution:
- "X is considered the leading authority" (by whom?)
- "The research was groundbreaking" (according to whom?)
- "The decision was widely criticized" (by whom? how widely?)

Indicators of biased attribution:
- Attributing one side's claims to named, credible sources while attributing the other side's claims vaguely ("critics say")
- Using asymmetric attribution verbs (one side "demonstrated" while the other "claimed")
- Attributing mainstream positions to individuals (making them seem like personal opinions) while stating fringe positions without attribution (making them seem like facts)

### 7. POV Fork

Content has been structured to separate positive and negative information about a subject into different sections or articles, creating the appearance of neutrality within each piece while the overall presentation is biased.

Indicators:
- An article about a person that is entirely positive, with a separate "Criticism of X" article
- Sections that are functionally advocacy pieces for different positions rather than integrated treatment
- Creation of parallel articles that cover the same topic from different editorial stances

### 8. Weasel Words and Peacock Terms

**Weasel words** create an impression of authority or consensus without identifying a source:
- "Some people say..."
- "It is widely believed that..."
- "Many scholars argue..."
- "Research has shown..."
- "Critics contend..."
- "It has been suggested that..."
- "Questions have been raised about..."

These are violations when they substitute for specific attribution. They are acceptable when the broad claim is supported by multiple cited sources.

**Peacock terms** are unsupported self-promotional language:
- "world-renowned," "leading," "prestigious"
- "one of the most important," "legendary"
- "widely regarded as," "iconic"

These are violations unless directly supported by cited independent sources.

### 9. Framing Bias

The overall structure, ordering, or framing of content implies a particular editorial stance even when individual sentences appear neutral.

Indicators:
- The lead paragraph or introduction frames the subject in a way that predisposes the reader
- Negative information is buried deep in the article while positive information leads
- Section headings that editorialize ("Groundbreaking discoveries" vs. "Research findings")
- The narrative arc of the article builds toward a particular conclusion
- Juxtaposition of facts that implies a causal or evaluative relationship not stated in sources

### 10. Geographic, Cultural, or Temporal Bias

Content assumes a particular geographic, cultural, or temporal perspective as default without acknowledging this framing.

Indicators:
- "The war" or "the election" without specifying which country's war or election
- Treating one country's legal or political norms as universal
- Using culturally specific value judgments as though they are universal
- Centering Western or English-language sources when the topic concerns other regions
- Presentism: judging historical events or figures by contemporary standards without noting this framing

## Detection Process

When evaluating text for NPOV violations, apply the following process:

1. **Read the full text first.** Individual sentences may appear neutral but create a biased impression in aggregate. Assess the overall effect before examining individual sentences.

2. **Identify the subject and its significant viewpoints.** Determine what the major perspectives on this topic are. Consider whether the text acknowledges all significant perspectives proportionately.

3. **Check each claim.** For each factual or evaluative claim, ask:
   - Is this attributed to a source, or stated as editorial fact?
   - If stated as fact, is it genuinely uncontested?
   - If attributed, is the attribution neutral in its verb choice and framing?

4. **Examine word choice.** Flag loaded verbs, editorializing adjectives/adverbs, value-laden labels, euphemisms, weasel words, and peacock terms.

5. **Assess proportionality.** Does the space given to each viewpoint roughly reflect its prominence in reliable sources? Are minority positions given disproportionate weight? Are majority positions understated?

6. **Look for omissions.** Is there readily available, well-sourced information representing a significant viewpoint that has been left out?

7. **Evaluate framing and structure.** Does the ordering, section structure, or narrative arc of the text nudge the reader toward a conclusion?

8. **Apply the inversion test.** Imagine reading the text from the perspective of someone who holds the opposite view on the subject. Would they find the presentation fair? If not, identify what specifically would strike them as biased.

## Severity Classification

When reporting violations, classify them by severity:

- **High:** The violation materially misleads the reader about the state of knowledge or the balance of opinion on the topic. Examples: stating contested claims as facts, omitting a major perspective entirely, giving equal weight to a fringe theory alongside scientific consensus.

- **Medium:** The violation nudges the reader toward a particular evaluation but does not fundamentally misrepresent the topic. Examples: loaded language in a few sentences, minor asymmetry in attribution, slightly disproportionate coverage of one perspective.

- **Low:** The violation is a stylistic issue that a careful reader would likely look past. Examples: a single peacock term, mild editorializing adverb, slightly imprecise weasel word.

## Important Caveats

- Not every instance of non-neutral language is a violation. Direct quotations may contain loaded language. Descriptions of clearly negative events (genocide, fraud) may use appropriately strong language that is factual, not editorial.

- Scientific consensus should be stated as fact, not hedged with false balance. Stating that "evolution is a scientific theory supported by extensive evidence" is neutral. Stating that "some scientists believe in evolution while others question it" is a violation (false balance).

- NPOV applies to how information is presented, not to whether the information itself is favorable or unfavorable to the subject. An article about a convicted criminal will contain predominantly negative information. This is not a violation if the information is factual, sourced, and presented without editorializing.

- Context matters. A word that is loaded in one context may be neutral in another. "Regime" is loaded when applied selectively to governments the writer disapproves of, but may be neutral in academic or historical contexts where it is the standard term.

- Tone is not the same as viewpoint balance. Text can have a measured, academic tone while still being biased through selective presentation of information. Conversely, text with strong language may be neutral if it accurately reflects the sources.
