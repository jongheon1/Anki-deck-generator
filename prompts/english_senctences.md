# Anki TSV Generator Template

This template helps generate English sentences for Anki decks in TSV format with customizable parameters.

## Basic Configuration

### CEFR Level Distribution
- A2: 20%
- B1: 50%
- B2: 20%
- C1: 10%

### Sentence Requirements
- Length: 15-25 words (strictly enforced)
- Diverse sentence patterns and structures
- Include practical phrasal verbs
- Avoid repetitive patterns

## TSV Format Structure

**Fields:** Sentence | Word | Pronunciation | Meaning | Synonym

1. **Sentence**: Complete English sentence (15-25 words)
2. **Word**: Key word
3. **Pronunciation**: British IPA pronunciation of Key word
4. **Meaning**: Clear English definition of the key word
5. **Synonym**: One synonym for the key word

I overslept this morning and missed my bus, so I had to take a taxi to work. oversleep [ˌəʊvəˈsliːp] To sleep longer than planned and be late for something. sleep in

## Contexts and Situations

Choose appropriate contexts for practical usage:

### Social Settings
- Friend conversations
- Family gatherings
- Social events
- Casual meetings

### Professional Settings
- Office environments
- Business meetings
- Client interactions
- Work presentations

### Public Services
- Hospitals/clinics
- Pharmacies
- Banks
- Government offices
- Post offices

### Transportation
- Buses/trains
- Airports
- Taxi/ride services
- Car rentals

### Commercial Settings
- Restaurants/cafes
- Shopping malls
- Supermarkets
- Hotels
- Tourist attractions

### Daily Life
- Home situations
- Neighborhood
- Emergency situations
- Personal care

## Pronunciation Guidelines

### British IPA Standards
- Use accurate British English pronunciation
- Clear vowel distinctions
- R-sound notation: use (r) for words ending in 'r'
- Stress marks: primary [ˈ] and secondary [ˌ]

### Common IPA Symbols
- /æ/ as in 'cat'
- /ɑː/ as in 'car'
- /ɪ/ as in 'bit'
- /iː/ as in 'bee'
- /ʊ/ as in 'book'
- /uː/ as in 'food'
- /e/ as in 'bed'
- /ɜː/ as in 'bird'
- /ə/ as in 'about'
- /ɔː/ as in 'saw'

## Word Selection Criteria

### Include
- Intermediate to advanced vocabulary
- Practical phrasal verbs
- Context-appropriate terms
- Professionally useful words
- Academic vocabulary (moderate level)

### Exclude
- Basic words (go, water, knife)
- Overly simple phrasal verbs (wake up, come in)
- Archaic or rarely used terms
- Highly technical jargon

## Customization Parameters

### Topic Focus (Choose one or more)
- [ ] Business English
- [ ] Travel English
- [ ] Academic English
- [ ] Daily conversation
- [ ] Medical English
- [ ] Technology
- [ ] Food and dining
- [ ] Shopping and services
- [ ] Transportation
- [ ] Emergency situations

### Difficulty Emphasis
- [ ] More A2-B1 focus (easier)
- [ ] More B2-C1 focus (harder)
- [ ] Balanced across all levels

### Special Requirements
- [ ] Include more phrasal verbs
- [ ] Focus on specific grammar patterns
- [ ] Emphasize collocations
- [ ] Include idiomatic expressions

## Output Requirements

### Format Rules
1. Use TAB separation (not commas)
2. No quotes around fields
3. No special characters between fields
4. Clean, copy-paste ready format

### File Naming Convention
`[topic]_[level]_anki_deck.tsv`

Examples:
- `business_intermediate_anki_deck.tsv`
- `travel_mixed_levels_anki_deck.tsv`
- `daily_conversation_anki_deck.tsv`

## Usage Instructions

1. Specify your desired topic/context
2. Choose CEFR level emphasis if different from default
3. Indicate any special requirements
4. Request specific number of sentences (default: 30)
5. Claude will generate the TSV file with appropriate naming

## Example Prompt Template

```
Create an Anki TSV file with [NUMBER] sentences focusing on [TOPIC/CONTEXT].
Use [LEVEL DISTRIBUTION if different from default].
Special requirements: [LIST ANY SPECIAL NEEDS].
Save as appropriately named TSV file.
```

## Quality Checklist

Before finalizing:
- [ ] All sentences 15-25 words
- [ ] CEFR levels distributed correctly
- [ ] British IPA pronunciation accurate
- [ ] Diverse sentence structures
- [ ] Practical, usable vocabulary
- [ ] Clean TSV formatting
- [ ] Appropriate file naming