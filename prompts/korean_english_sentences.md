# Anki TSV Generator: 2-Column Simple Mode (School & Interview Add-on)

This template generates sentence pairs for "Korean to English" speaking practice.
Output must be strictly 2 columns separated by a TAB.

## Basic Configuration

### CEFR Level Distribution
- A2 (Basic): 40% (Simple sentences for speed)
- B1 (Intermediate): 60% (Compound sentences for expression)

### Sentence Requirements
- **Length**: 7-15 words (Optimized for one-breath speaking)
- **Style**: Natural, spoken English
- **No Complex Jargon**: Focus on sentence structure, not difficult technical words.

## TSV Format Structure (Strict)

**Fields:** Korean | English

1. **Korean**: Natural Korean thought/sentence
2. **English**: Corresponding English sentence

**Example:**
이번 학기에 전공 수업 몇 개 들어?	How many major classes are you taking this semester?
제 강점은 새로운 기술을 빨리 배운다는 거예요.	My strength is that I can learn new technologies quickly.

## Contexts (Selectable)

1. **Daily Life**: Hobbies, Weekend plans, Food, Travel
2. **Office Life**: Status updates, Asking for help, Scheduling
3. **School Life (New)**:
   - Group projects & Teamwork
   - Asking professors/TAs questions
   - Campus life & Exchange student situations
4. **Job Interview (New)**:
   - Self-introduction (Simple)
   - Describing projects (STAR method basics)
   - Talking about strengths/weaknesses
   - Asking the interviewer questions
   

## Output Requirements

### Format Rules
1. **Strictly 2 Columns**: [Korean] [TAB] [English]
2. **NO Header**: Do not include "Korean | English" at the top.
3. **NO Numbering**: Do not add "1.", "2." at the start.
4. **NO Extra text**: Just the raw TSV data in a code block.

## Prompt Template to use

"Create [NUMBER] sentence pairs about [CONTEXT].
Level: A2/B1 mix.
Format: Korean [TAB] English
Keep the Korean natural."