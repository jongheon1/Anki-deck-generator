# Academic Paper Anki TSV Generator

This template creates effective Anki decks in TSV format from research papers using Nielsen's spaced repetition principles and a three-layer learning structure optimized for deep academic understanding.

## Core Learning Philosophy

Based on Michael Nielsen's "Augmenting Long-term Memory" principles:
- **Atomic understanding**: Break complex concepts into fundamental components
- **Elaborative encoding**: Create rich associations between ideas
- **Avoid orphan knowledge**: Connect new concepts to existing framework
- **Hierarchical learning**: Build from basic facts to integrated understanding

## Content Selection Criteria

### Priority Elements (Must Include)
- **Problem statements**: What challenges did authors identify?
- **Solution approaches**: How did they address these problems?
- **Key innovations**: What novel contributions were made?
- **Design principles**: What fundamental ideas guide the system?
- **Trade-offs and limitations**: What compromises were necessary?
- **Results and implications**: What did they achieve and why it matters?

### Sentence Selection Guidelines
- Choose sentences that contain core technical concepts
- Prefer sentences explaining causality or relationships
- Include direct quotes that capture essential insights
- Focus on sentences that answer "why" and "how" questions
- Avoid purely descriptive or statistical sentences

## Question Types for Deep Understanding

### Conceptual Relationship Questions
- "How does [concept A] relate to [concept B] in this system?"
- "What principle underlies this design decision?"
- "Why was this approach chosen over alternatives?"

### Problem-Solution Questions
- "What problem does this sentence identify?"
- "How does this design solve the stated challenge?"
- "What trade-offs are implicit in this statement?"

### Implication Questions
- "What broader implications does this have for [field]?"
- "How does this contribute to the paper's main thesis?"
- "What limitations does this approach suggest?"

## Academic Paper Analysis Framework

### Structure-Based Content Extraction

**Abstract/Introduction**: Focus on problem definition and contribution claims
**Related Work**: Extract key differentiators and positioning
**Methodology**: Capture design principles and novel approaches  
**Results**: Highlight significant findings and their implications
**Discussion/Conclusion**: Include limitations, future work, and broader impact

### Technical Depth Levels

**Level 1 - Foundational** (30% of cards)
- Basic terminology and definitions
- Core system components
- Fundamental principles

**Level 2 - Mechanistic** (40% of cards)  
- How systems work together
- Process flows and interactions
- Design rationale

**Level 3 - Analytical** (30% of cards)
- Trade-offs and limitations
- Comparative advantages
- Broader implications

## Note Generation Guidelines

### Adaptive Quantity Based on Paper Characteristics

**Short Papers (4-8 pages)**: 15-25 notes
**Standard Papers (8-12 pages)**: 25-40 notes  
**Long Papers (12+ pages)**: 40-60 notes

**Density Factors:**
- High technical novelty: +20% notes
- Foundational/survey papers: +30% notes
- Incremental improvements: -20% notes
- Heavy mathematical content: Focus on key theorems/proofs

### Field-Specific Guidelines

**Original_Sentence Field**
- Extract complete, meaningful sentences (not fragments)
- Preserve exact wording from paper
- Choose sentences that can stand alone contextually
- Avoid sentences requiring extensive background from previous paragraphs

**Contextual_Question Field**
- Create questions that probe understanding, not just recall
- Use open-ended questions that require synthesis
- Avoid questions answerable by simple keyword matching
- Focus on "why," "how," and "what does this mean" questions

**Core_Concept Field**
- Identify the single most important technical term or principle
- Use precise terminology from the field
- Keep to 1-3 words when possible
- Choose concepts that connect to broader themes

**Explanation Field**
- Provide clear, jargon-free explanations
- Include enough context for understanding
- Keep concise but complete (1-2 sentences maximum)
- Define technical terms that might be unfamiliar

**Paper_Significance Field**
- Connect to paper's main contributions
- Explain why this concept matters in the research context
- Link to broader implications for the field
- Highlight how it relates to the problem being solved

## Output Specifications

### TSV Format Structure

**Fields:** Original_Sentence | Contextual_Question | Core_Concept | Explanation | Paper_Significance

1. **Original_Sentence**: Key sentence extracted directly from the paper (preserved exactly as written)
2. **Contextual_Question**: Probing question that tests understanding of the sentence's deeper meaning
3. **Core_Concept**: The main technical term, principle, or idea being highlighted
4. **Explanation**: Clear, concise explanation of the core concept
5. **Paper_Significance**: Why this concept matters within the paper's broader context and contribution

### TSV Format Requirements
- Use TAB separation between fields only
- No quotes around fields unless content contains tab characters
- Maintain consistent field order throughout file
- Clean, importable format for Anki with proper UTF-8 encoding

### Example Output Format

```
The system calls to do I/O are designed to eliminate differences between various devices and styles of access.	What design principle does this sentence illustrate?	Unified interface design	A design approach where different components are accessed through the same interface, hiding implementation complexity	Demonstrates UNIX's key innovation of treating all devices as files, which simplified programming and improved system consistency
```

### Card Template Design

**Front Side:**
- Original_Sentence (displayed as context)
- Contextual_Question (main prompt for active recall)

**Back Side:**
- Original_Sentence + Contextual_Question (repeated for reference)
- Core_Concept (highlighted as the key term)
- Explanation (detailed understanding)
- Paper_Significance (broader context and importance)

**Design Principles:**
- Modern, minimal, clean aesthetic
- Clear visual hierarchy with proper spacing
- Mobile-responsive layout
- Professional color scheme suitable for academic content
- Emphasis on readability and comprehension

### File Naming Convention
`[first_author_surname]_[publication_year]_[key_topic]_anki.tsv`

Examples:
- `ritchie_1974_unix_filesystem_anki.tsv`
- `lamport_1998_distributed_consensus_anki.tsv`


## Quality Assurance Checklist

**Content Quality**
- [ ] Each original sentence is meaningful and self-contained
- [ ] Questions probe understanding, not just recall
- [ ] Core concepts are precisely identified
- [ ] Explanations are clear and accessible
- [ ] Paper significance connects to broader research context

**Learning Effectiveness**
- [ ] Cards build hierarchically from simple to complex
- [ ] Related concepts are cross-referenced through questions
- [ ] No orphan cards (isolated from main themes)
- [ ] Questions encourage elaborative thinking
- [ ] Balance between factual and conceptual understanding

## Prompt Template Usage

```
Analyze the attached research paper and create an Anki TSV deck using the five-field structure: Original_Sentence | Contextual_Question | Core_Concept | Explanation | Paper_Significance

Paper focus: [SPECIFY if particular sections are priority]
Emphasis level: [FOUNDATIONAL/MECHANISTIC/ANALYTICAL if different from default balance]
Special requirements: [Any specific concepts or themes to emphasize]

Generate an appropriately sized deck based on paper length and technical density, following the academic paper analysis framework.
```