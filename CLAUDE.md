# Anki Content Generator

This project generates customized Anki decks in TSV format with matching card templates from various source materials using specialized generation prompts.

## Project Purpose

Transform diverse learning materials (academic papers, documents, texts) into effective Anki spaced repetition cards through:
- **Prompt-driven generation**: Different prompts for different content types and learning goals
- **Source-based processing**: Extract meaningful content from provided materials
- **Automated formatting**: Generate both TSV data and matching card templates
- **Flexible workflows**: Support multiple learning domains and content types

## Project Structure

```
├── prompts/          # Generation templates for different content types
├── sources/          # Source materials (PDFs, texts, documents)
├── results/          # Generated TSV files for Anki import
└── card_templates/   # Generated Anki card templates (HTML/CSS)
```

### Directory Functions

**prompts/**
Contains specialized generation templates, each optimized for specific content types:
- Define field structures for TSV output
- Specify content extraction strategies
- Set quality standards and formatting rules
- Provide domain-specific guidelines

**sources/**
Storage for source materials to be processed:
- Academic papers (PDF)
- Text documents
- Web articles
- Any readable content format

**results/**
Generated TSV files ready for Anki import:
- Tab-separated format compatible with Anki
- Named according to content and prompt type
- Multiple field structures based on chosen prompt

**card_templates/**
Generated Anki card templates (HTML/CSS/JS):
- Front and back templates
- Styling definitions
- Instructions for Anki setup
- Optimized for the corresponding TSV structure

## Available Generation Prompts

### academic_paper.md
**Purpose**: Extract key concepts from research papers for deep academic understanding
**Fields**: Original_Sentence | Contextual_Question | Core_Concept | Explanation | Paper_Significance
**Best for**: Research papers, technical documents, scholarly articles
**Output**: Analytical cards focusing on comprehension and critical thinking

### english_sentences.md
**Purpose**: Generate practical English vocabulary learning sentences
**Fields**: Sentence | Word | [Pronunciation] | meaning | Synonym
**Best for**: Language learning, vocabulary building
**Output**: CEFR-leveled sentences with pronunciation guides

## Usage Workflow

### Basic Usage Pattern
```
"Generate cards from [SOURCE_FILE] using [PROMPT_FILE] approach"
```

### Example Commands
```
"unix.pdf 파일을 바탕으로 academic_paper.md에 따라서 TSV와 TXT를 생성해줘"

"Create Anki cards from research_paper.pdf using the academic_paper.md template"

"Generate vocabulary cards from article.txt following english_sentences.md format"
```

### Step-by-Step Process
1. **Source Preparation**: Place source material in `sources/` directory
2. **Prompt Selection**: Choose appropriate prompt from `prompts/` directory
3. **Generation Request**: Request processing using the specified prompt
4. **Style Selection** (Interactive Mode):
   - Generate 2-3 sample cards with different style variations
   - Present examples to user showing different approaches
   - Ask user to select preferred style or provide custom preferences
   - Proceed with full generation using selected style
5. **Output Generation**:
   - TSV file created in `results/`
   - Card template created in `card_templates/` (only if template doesn't already exist)
6. **Anki Import**: Use generated template and import TSV data

### Interactive Style Selection

**IMPORTANT**: Before generating the full TSV file, follow this interactive workflow:

1. **Generate Style Variations**
   - Create 2-3 example cards from the source material
   - Each example should use a different stylistic approach while following the prompt's field structure
   - Variations can differ in:
     - Tone (formal/casual, academic/practical)
     - Complexity level (beginner/intermediate/advanced)
     - Question style (direct/contextual, simple/analytical)
     - Content focus (breadth vs. depth, theory vs. application)

2. **Present Options to User**
   - Show the example variations clearly
   - Explain the characteristics of each style
   - Use the AskUserQuestion tool to let user select their preferred approach
   - Option to customize or combine styles

3. **Generate Full Content**
   - Once style is confirmed, proceed with generating all cards
   - Maintain consistency with the selected style throughout
   - Apply the style preferences to all generated content

**Example Style Variations**:
```
Style A (Academic/Formal): Deep conceptual focus, precise terminology
Style B (Practical/Applied): Real-world examples, simpler language
Style C (Balanced): Mix of theory and application, moderate complexity
```

## Output Specifications

### TSV Format Requirements
- **Field Separation**: TAB characters only (not commas)
- **Encoding**: UTF-8
- **Quotes**: No quotes around fields
- **Consistency**: Maintain field order throughout file
- **Compatibility**: Direct Anki import ready

### Card Template Requirements
- **Complete Templates**: Front, back, and styling sections
- **Field Mapping**: Clear correspondence with TSV fields
- **Setup Instructions**: Step-by-step Anki configuration guide
- **Responsive Design**: Mobile and desktop optimized
- **Professional Styling**: Clean, readable, consistent appearance
- **Template Reuse**: Use existing template if it matches the prompt name, create new only if missing

### File Naming Conventions

**TSV Files**: `[source_name]_[prompt_type]_[date/id].tsv`
- `unix_paper_academic_2024.tsv`
- `business_vocabulary_english_sentences.tsv`
 
**Template Files**: `[prompt_name].txt` (matches prompt filename)
- `academic_paper.txt` (from `prompts/academic_paper.md`)
- `english_sentences.txt` (from `prompts/english_sentences.md`)

**Template Generation Logic**:
- Check if `card_templates/[prompt_name].txt` exists
- If exists: Skip template creation (reuse existing)
- If missing: Generate new template based on prompt specifications

## Quality Assurance

### Content Standards
- [ ] Source material accurately represented
- [ ] Prompt guidelines followed precisely
- [ ] Field requirements met
- [ ] Appropriate difficulty/complexity level

### Technical Standards
- [ ] Clean TSV formatting (no parsing errors)
- [ ] Template compatibility with Anki
- [ ] Proper UTF-8 encoding
- [ ] Consistent field mapping
- [ ] File naming conventions followed

### Learning Effectiveness
- [ ] Cards test understanding, not just recall
- [ ] Progressive difficulty when applicable
- [ ] Contextually relevant examples
- [ ] Clear, unambiguous questions/prompts
- [ ] Balanced content distribution

## Extending the System

### Adding New Prompts
1. Create new `.md` file in `prompts/` directory
2. Define field structure and content guidelines
3. Specify extraction strategies for the content type
4. Include quality standards and examples
5. Test with representative source materials

### Supported Content Types
- **Academic**: Research papers, theses, technical reports
- **Language Learning**: Texts, articles, dialogues
- **Professional**: Training materials, documentation
- **General Knowledge**: Books, articles, reference materials

## Generation Priority Rules

**IMPORTANT**: When processing generation requests:

1. **Specific Prompt Rules Override General Rules**
   - Individual prompt files (e.g., `academic_paper.md`, `english_sentences.md`) contain detailed, specialized guidelines
   - These specific prompt rules ALWAYS take precedence over general guidelines in this CLAUDE.md
   - Follow the exact field structures, formatting requirements, and content strategies defined in the chosen prompt

2. **Interactive Style Selection First**
   - **NEVER generate the full TSV immediately** upon receiving a generation request
   - ALWAYS start by creating 2-3 style-varied example cards
   - Use AskUserQuestion tool to present options and get user preference
   - Only proceed with full generation after user confirms their preferred style
   - This applies to ALL new generation requests (does not apply to modifications of existing files)

3. **Processing Order**
   - Load and prioritize the specific prompt template first
   - Read source material to understand content
   - Generate 2-3 style variations and present to user
   - Wait for user style selection
   - Check for existing card template: `card_templates/[prompt_name].txt`
   - Generate full TSV file according to prompt specifications and selected style
   - Create card template only if it doesn't exist
   - Use this CLAUDE.md only for general workflow and project structure guidance

4. **Template Management**
   - Template filename must match prompt filename (without .md extension)
   - Reuse existing templates to maintain consistency across generations
   - Only create new templates when prompt requires different field structure or design

## Integration Notes

This system is designed to work with Claude Code's file processing capabilities:
- Automatic prompt loading and interpretation
- Source file analysis and content extraction
- Multi-format output generation
- Quality validation and formatting