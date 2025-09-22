# Academic Paper Anki TSV Generator

This template creates effective Anki decks in TSV format from research papers using Nielsen's spaced repetition principles with a streamlined two-field structure for authentic contextual learning.

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


## Field-Specific Guidelines

**Original_Sentence Field**
- Extract complete, meaningful sentences that can stand alone
- Preserve exact wording from paper
- Choose sentences with substantial technical or conceptual content
- Select sentences that represent key insights or turning points in the argument

**Surrounding_Context Field**  
- Include 1-3 sentences from immediately before or after the target sentence
- Choose context that directly illuminates or clarifies the main sentence
- Preserve the author's exact wording to maintain authenticity
- Focus on content that shows the logical flow of the author's reasoning
- Include context that helps disambiguate technical terms or concepts

## Output Specifications

### TSV Format Structure

**Fields:** Original_Sentence | Surrounding_Context

1. **Original_Sentence**: Key sentence extracted directly from the paper (preserved exactly as written)
2. **Surrounding_Context**: Relevant sentences from immediately before/after that provide essential context and clarification

### TSV Format Requirements
- Use TAB separation between fields only
- No quotes around fields unless content contains tab characters
- Maintain consistent field order throughout file
- Clean, importable format for Anki with proper UTF-8 encoding

### Example Output Format

```
The system calls to do I/O are designed to eliminate differences between various devices and styles of access.	There is no distinction between "random" and sequential I/O, nor is any logical record size imposed by the system. The size of an ordinary file is determined by the highest byte written on it; no predetermination of the size of a file is necessary or possible.
```

### Card Template Design

**Front Side:**
- Original_Sentence (displayed as context)

**Back Side:**
- Original_Sentence(repeated for reference)
- Surrounding_Context


### File Naming Convention
`[first_author_surname]_[publication_year]_[key_topic]_anki.tsv`

Examples:
- `ritchie_1974_unix_filesystem_anki.tsv`
- `lamport_1998_distributed_consensus_anki.tsv`

## Quality Assurance Checklist

**Content Quality**
- [ ] Each original sentence is meaningful and contains substantial technical content
- [ ] Surrounding context directly clarifies or expands the main sentence
- [ ] Context preserves author's reasoning flow
- [ ] No sentences that require extensive external background
- [ ] Context helps disambiguate technical concepts

**Learning Effectiveness**
- [ ] Cards build hierarchically from simple to complex concepts
- [ ] Related concepts naturally connect through context
- [ ] No orphan cards isolated from main themes
- [ ] Context encourages deeper understanding of author's logic
- [ ] Balance across foundational, mechanistic, and analytical levels

## Prompt Template Usage

```
Analyze the attached research paper and create an Anki TSV deck using the two-field structure: Original_Sentence | Surrounding_Context

Paper focus: [SPECIFY if particular sections are priority]
Emphasis level: [FOUNDATIONAL/MECHANISTIC/ANALYTICAL if different from default balance]
Special requirements: [Any specific concepts or themes to emphasize]

Generate an appropriately sized deck based on paper length and technical density, following the academic paper analysis framework. Focus on extracting sentences with substantial technical content and providing authentic surrounding context that illuminates the author's reasoning.
```