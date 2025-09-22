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

This template structure ensures you provide all necessary information while clearly specifying your learning objectives and preferred approach to the material.