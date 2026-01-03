# Anki TSV Generator: 2026 TOEFL Reading - Complete the Words

Generate academic sentences with single word blanks for vocabulary practice.
Each card: **[Sentence with ___ ]** → **[Answer + Related words]**

## 1. Configuration

### Difficulty Level
- **Target 80** (High-frequency academic words, clear context)
- **Target 90** (Academic Word List, moderate context clues)
- **Target 100+** (Advanced academic vocabulary, subtle context)

### Word Type Focus
- **Verbs** (academic actions: demonstrate, indicate, enhance, etc.)
- **Nouns** (abstract concepts: phenomenon, implication, framework, etc.)
- **Adjectives** (descriptive academic: substantial, significant, prevalent, etc.)
- **Mixed** (balanced distribution across word types)

## 2. TSV Format Structure (Strict)

**Fields:** Question | Answer

### Card Format

**Front (Question):**
- One complete academic sentence (15-30 words)
- Exactly ONE blank marked as ___
- Context clues should guide to answer but not make it obvious

**Back (Answer):**
```
Answer: [correct word]

Synonyms: [2-3 synonyms]
Collocations: [2-3 common phrases with this word]
Note: [brief usage tip or confusing similar words]
```

## 3. Sentence Requirements

### Academic Style
- Use formal academic register
- Include domain-neutral academic content (science, social science, humanities)
- Sentence must be complete and grammatically correct
- Context clues in sentence should narrow down to correct word family/meaning

### Blank Placement Strategy
- Place blank at KEY position (not articles, prepositions)
- Blank should test vocabulary knowledge, not just grammar
- Surrounding words should provide semantic context
- Avoid blanks that have multiple equally valid answers

## 4. Answer Format Requirements

### Components (Always Include)

1. **Answer:** The single correct word
2. **Synonyms:** 2-3 words with similar meaning in this context
3. **Collocations:** 2-3 phrases where this word commonly appears
4. **Note:** One of the following:
   - Common confusing words (e.g., "Not 'affect' - that's a verb")
   - Usage tip (e.g., "Formal academic writing")
   - Word family (e.g., "Noun form: significance")

### Formatting
- Use line breaks (\n) between sections
- Keep each section concise (1 line each)
- No bullet points, use simple text

## 5. Output Requirements

### Format
1. **Strictly 2 Columns**: [Question] [TAB] [Answer]
2. **NO Header Row**: Start directly with data
3. **NO Code Blocks**: Raw text only
4. **15-20 Cards**: Mix of word types and difficulty

### Quality Checks
- ✓ Only ONE blank per sentence
- ✓ Context provides reasonable clues
- ✓ Answer section is complete (all 4 components)
- ✓ Synonyms are appropriate for the context
- ✓ Collocations are authentic and useful

## 6. Examples

### Example 1: Verb (Target 90)
```
The study clearly ___ that regular exercise improves cognitive function in elderly adults.	Answer: demonstrates\n\nSynonyms: shows, indicates, reveals\nCollocations: clearly demonstrates, study demonstrates, research demonstrates\nNote: Academic writing prefers "demonstrates" over "shows" for research findings.
Recent research ___ a strong correlation between sleep quality and academic performance among college students.	Answer: indicates\n\nSynonyms: suggests, shows, reveals\nCollocations: research indicates, data indicates, evidence indicates\nNote: "Indicates" implies indirect evidence, unlike "proves" which is stronger.
```

### Example 2: Noun (Target 100+)
```
The rapid ___ of artificial intelligence has raised important ethical questions about privacy and human autonomy.	Answer: proliferation\n\nSynonyms: expansion, spread, growth\nCollocations: rapid proliferation, proliferation of technology, nuclear proliferation\nNote: Formal term often used for rapid/uncontrolled increase, especially of technology or weapons.
This ___ has been observed across multiple cultures, suggesting it may be a universal human trait rather than culturally specific.	Answer: phenomenon\n\nSynonyms: occurrence, pattern, trend\nCollocations: natural phenomenon, widespread phenomenon, observed phenomenon\nNote: Plural is "phenomena" - common mistake to use "phenomenons".
```

### Example 3: Adjective (Target 90)
```
The government's new environmental policies have had a ___ impact on reducing carbon emissions nationwide.	Answer: significant\n\nSynonyms: substantial, considerable, notable\nCollocations: significant impact, significant difference, significant increase\nNote: More formal than "big" or "large" in academic writing.
Sleep deprivation is ___ among college students, with surveys showing over 60% regularly get less than seven hours per night.	Answer: prevalent\n\nSynonyms: common, widespread, frequent\nCollocations: highly prevalent, increasingly prevalent, prevalent condition\nNote: Used for conditions/situations that are widespread in a population.
```

### Example 4: Mixed Difficulty
```
Scientists have developed a new ___ for analyzing complex genetic data more efficiently than previous methods.	Answer: framework\n\nSynonyms: system, structure, model\nCollocations: theoretical framework, analytical framework, conceptual framework\nNote: Common in academic writing to describe systematic approaches or structures.
The researcher's findings ___ previous assumptions about how children acquire language skills.	Answer: challenge\n\nSynonyms: question, dispute, contradict\nCollocations: findings challenge, challenge assumptions, challenge conventional wisdom\nNote: Academic verb meaning "to question the validity of" - not physical challenge.
The decline in bee populations poses a ___ threat to global food security and ecosystem stability.	Answer: substantial\n\nSynonyms: significant, considerable, major\nCollocations: substantial threat, substantial evidence, substantial amount\nNote: Stronger than "considerable" but less dramatic than "severe".
```

---

**Usage Note**: Generate 15-20 cards per session. Mix word types (verbs, nouns, adjectives) and difficulty levels. Focus on Academic Word List vocabulary that appears frequently in TOEFL reading passages.