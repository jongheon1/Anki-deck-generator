# Academic Book Anki TSV Generator

This template creates effective Anki decks in TSV format from academic and technical books using Nielsen's spaced repetition principles with a streamlined two-field structure for conceptual understanding and contextual learning.


## Core Learning Philosophy

Based on Michael Nielsen's "Augmenting Long-term Memory" principles:
- **Atomic understanding**: Break complex concepts into fundamental components
- **Elaborative encoding**: Create rich associations between ideas
- **Avoid orphan knowledge**: Connect new concepts to existing framework
- **Hierarchical learning**: Build from basic facts to integrated understanding


## Source Material Requirements

### Essential Information Needed
- **Book Title**: Full title and subtitle if applicable
- **Author(s)**: Primary author(s) and publication year
- **Table of Contents**: Complete chapter titles and major subsection headings
- **Book Type**: Textbook, reference manual, theoretical work, practical guide
- **Target Audience**: Undergraduate, graduate, professional, general audience

### Optional Enhancements
- Brief description of book's main approach or methodology
- Specific chapter focus if targeting particular sections
- Prerequisites or background knowledge assumed


## Content Selection Strategy

### Book Analysis Framework

**Foundational Level** (40% of cards)
- Core terminology and definitions
- Basic principles and concepts
- Fundamental building blocks

**Application Level** (35% of cards)
- Techniques and methods
- Problem-solving approaches
- Practical implementations

**Integration Level** (25% of cards)
- How concepts connect together
- Advanced applications
- Limitations and trade-offs

### Concept Prioritization

**High Priority Elements**
- Concepts that appear in multiple chapters
- Fundamental principles underlying the subject
- Techniques with broad applicability
- Key insights that change understanding

**Medium Priority Elements**
- Chapter-specific methods
- Detailed implementations
- Historical context and background

**Lower Priority Elements**
- Highly specialized applications
- Tangential discussions
- Pure reference material


## Field Construction Guidelines

### Core_Concept Field (15-30 words)
- State the principle, technique, or idea clearly and precisely
- Use the author's terminology when possible
- Focus on what the concept IS rather than what it does
- Avoid unnecessary qualifiers or hedging language
- Include key technical terms that students should learn

### Context Field (20-40 words)
- Explain WHY this concept is important or useful
- Show HOW it connects to other concepts in the book
- Indicate WHEN or WHERE this concept applies
- Highlight what understanding this enables or prevents
- Connect to the book's overall learning objectives


## Book Type Adaptations

### Technical/Engineering Books
- Emphasize practical applications and implementation details
- Connect theoretical concepts to real-world problems
- Include performance considerations and trade-offs

### Mathematical/Theoretical Books
- Focus on logical progression and proof techniques
- Emphasize prerequisite concepts and building relationships
- Include intuitive explanations alongside formal definitions

### Computer Science Books
- Balance algorithmic understanding with implementation concerns
- Connect abstract concepts to concrete examples
- Emphasize complexity analysis and design principles

### Business/Management Books
- Focus on frameworks and decision-making tools
- Emphasize practical application scenarios
- Connect concepts to organizational contexts

### Literature Books
- Focus on thematic elements, character development, and narrative techniques
- Connect literary devices to their effects on meaning and reader experience
- Emphasize cultural and historical context that influences interpretation

### Philosophy Books
- Emphasize logical argumentation and conceptual distinctions
- Connect abstract concepts to concrete examples and thought experiments
- Focus on how ideas build upon or challenge previous philosophical positions

### History Books
- Connect events to broader historical patterns and causation
- Emphasize the significance of developments within their temporal context
- Focus on how historical understanding shapes contemporary perspectives

### Social Science Books
- Balance theoretical frameworks with empirical evidence
- Connect research findings to practical social implications
- Emphasize methodological approaches and their limitations


## Note Generation Guidelines

### Learning Mode-Based Quantity

**Deep Study Mode** (Complete mastery and understanding)
- 30-50 cards per chapter
- Focus on comprehensive concept coverage including definitions, applications, and connections
- Include both foundational elements and advanced implications
- Suitable for core subjects in your field or essential reference materials

**Survey Mode** (Overview and general familiarity)
- 15-25 cards per chapter
- Emphasize major themes, key frameworks, and central arguments
- Cover breadth rather than depth, focusing on concepts that appear multiple times
- Ideal for exploring new fields or getting familiar with adjacent disciplines

**Review Mode** (Reinforcing previously read material)
- 10-20 cards per chapter
- Concentrate on easily forgotten details and crucial connections between concepts
- Highlight insights that were particularly valuable or challenging during initial reading
- Perfect for maintaining knowledge of important books over time

### Content Density Adjustments

**High-density content** requires full recommended quantities since every page contains essential information that builds upon previous concepts.

**Medium-density content** works well with about eighty percent of the recommended range, allowing you to focus on the most substantial ideas while skipping purely illustrative material.

**Low-density content** benefits from about sixty percent of the recommended range, concentrating on the core insights while avoiding repetitive examples or extended anecdotes.


## Output Specifications

### TSV Format Structure

**Fields**: Core_Concept | Context

1. **Core_Concept**: Fundamental principle, technique, or idea presented concisely (15-30 words)
2. **Context**: Why this concept matters, how it connects to other ideas, or what it enables (20-40 words)

### TSV Format Requirements
- Use TAB separation between fields only
- No quotes around fields unless content contains tab characters
- Maintain consistent field order throughout file
- Clean, importable format for Anki with proper UTF-8 encoding

### Example Output Format

```
Loop unrolling processes multiple elements per iteration to reduce loop control overhead.	This optimization builds on eliminating loop inefficiencies and prepares students for understanding advanced parallelism techniques.
```

```
Amdahl's Law quantifies the maximum speedup achievable when optimizing only portions of a program.	This mathematical principle explains why profiling is essential for identifying performance bottlenecks in real applications.
```

### Card Template Design

**Front Side:**
- Core_Concept

**Back Side:**
- Core_Concept(repeated for reference)
- Context


### File Naming Convention
`[author_surname]_[publication_year]_[key_topic]_anki.tsv`

Examples:
- `bryant_2015_csapp_performance_anki.tsv`
- `cormen_2009_algorithms_sorting_anki.tsv`
- `tanenbaum_2014_networks_protocols_anki.tsv`


## Quality Assurance Checklist

**Content Quality**
- [ ] Each core concept is clearly stated and self-contained
- [ ] Context explains significance within the book's framework
- [ ] Technical terminology is used accurately
- [ ] Concepts build logically from simple to complex
- [ ] No orphan concepts disconnected from main themes

**Learning Effectiveness**
- [ ] Cards cover essential concepts comprehensively
- [ ] Context helps students understand practical relevance
- [ ] Related concepts are implicitly connected through context
- [ ] Balance between foundational, application, and integration levels
- [ ] Appropriate density for book type and complexity


## Prompt Template Usage

```
Create an Anki TSV deck from the provided book information using the two-field structure: Core_Concept | Context

Book Information:
- Title: [FULL TITLE with subtitle if applicable]
- Author(s): [AUTHOR NAME(S)] ([PUBLICATION YEAR])
- Table of Contents: [COMPLETE CHAPTER TITLES AND MAJOR SUBSECTIONS]
- Book Type: [Textbook/Reference Manual/Theoretical Work/Literature/Philosophy/etc.]
- Target Audience: [Undergraduate/Graduate/Professional/General]

Learning Parameters:
- Mode: [DEEP STUDY/SURVEY/REVIEW MODE - specify your learning goal]
- Focus: [FULL BOOK or SPECIFIC CHAPTERS/SECTIONS]
- Content Density: [HIGH/MEDIUM/LOW - adjust card quantity accordingly]
- Special Emphasis: [FOUNDATIONAL/APPLICATION/INTEGRATION if different from default 40/35/25 balance]

Additional Requirements: [Any specific themes, difficulty preferences, or learning objectives]

Generate an appropriately sized deck following the learning mode guidelines and book type adaptations, with strict adherence to word limits: Core_Concept (15-30 words), Context (20-40 words).
```

### Usage Examples

**For Deep Study of Technical Book:**
```
Book: Computer Systems: A Programmer's Perspective by Bryant & O'Hallaron (2015)
Mode: DEEP STUDY MODE
Focus: Chapter 5 - Optimizing Program Performance
Content Density: HIGH
Special Emphasis: Balance foundational concepts with practical applications
```

**For Survey of Philosophy:**
```
Book: Justice: What's the Right Thing to Do? by Michael Sandel (2009)
Mode: SURVEY MODE  
Focus: FULL BOOK
Content Density: MEDIUM
Special Emphasis: Focus on major ethical frameworks and their applications
```

**For Review of Previously Read Literature:**
```
Book: Pride and Prejudice by Jane Austen (1813)
Mode: REVIEW MODE
Focus: FULL BOOK
Content Density: LOW
Special Emphasis: Character development and major themes only
```