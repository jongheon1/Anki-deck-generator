# Anki Generator: TOEFL Listening - Dictation Practice

## Purpose
Generate English sentences for listening comprehension practice.
User listens via TTS, transcribes the sentence, then checks the answer.

## Configuration

### CEFR Level
- B2-C1 (TOEFL academic level)

### Sentence Specs
- **Length**: 12-20 words (TOEFL average sentence length)
- **Style**: Academic lecture/discussion style
- **Natural speech**: Include discourse markers, academic transitions

### Topics (Rotate)
1. **Computer Science**: Algorithms, Operating Systems, Networks, Databases, Software Engineering
2. **Biology**: Evolution, Ecology, Genetics, Cell Biology, Marine Biology
3. **Psychology**: Cognitive processes, Development, Social psychology, Behavioral studies
4. **Art History**: Movements, Artists, Techniques, Cultural context
5. **Environmental Science**: Climate, Ecosystems, Conservation, Sustainability
6. **Astronomy**: Planets, Stars, Galaxies, Space exploration
7. **Geology**: Earth structure, Rocks, Plate tectonics, Natural disasters
8. **History**: Ancient civilizations, Historical events, Cultural developments
9. **Economics**: Markets, Trade, Economic systems, Business concepts

## Sentence Types (Mix Naturally)

1. **Main Idea** (30%): Topic sentences, thesis statements
2. **Detail/Example** (40%): Supporting evidence, specific examples, data
3. **Transition/Opinion** (20%): Professor's stance, discourse markers, hedging
4. **Function** (10%): Instructions, assignments, procedural info

## Output Format

**Strict Rules:**
- One sentence per line
- English ONLY (no Korean, no tags, no numbering)
- No header, no extra text
- Just plain sentences in a code block

**Example Output:**
```
Virtual memory allows each process to have its own isolated address space.
Mitochondria generate ATP through a process called oxidative phosphorylation.
The Impressionist movement began in France during the late nineteenth century.
Climate change is affecting migration patterns of various bird species.
```