# Anki TSV Generator: 2026 TOEFL Chain Mode

Generate sequential sentence chains for TOEFL practice.
Each card flows: **[Previous Context]** → **[Next Sentence]**

## 1. Configuration (Select One Per Category)

### Topic Selection
Use common TOEFL Speaking/Writing topics covering academic and daily life scenarios.

### Task Type
- **Speaking Interview** (3-4 sentences, 50-70 words, conversational responses)
- **Writing Email** (6-10 sentences, 100-150 words, appropriate formality)
- **Writing Academic Discussion** (5-8 sentences, 100-150 words, academic tone)

### Difficulty Level
- **Target 80** (Simple structure, common vocab, clear and direct)
- **Target 90** (Varied structure, academic vocab, natural flow)
- **Target 100+** (Complex syntax, precise diction, sophisticated reasoning)

## 2. TSV Format Structure (Strict)

**Fields:** Stimulus | Response

### Card Breakdown

**Speaking Interview (3-4 cards):**
```
Card 1: Question → Answer + Reason
Card 2: Answer + Reason → Example/Detail
Card 3: Example/Detail → Conclusion
```

**Writing Email (6-10 cards):**
```
Card 1: Situation → Greeting + Purpose
Card 2: Greeting + Purpose → Main point 1
Card 3: Main point 1 → Main point 2
Card 4-6: Additional details/explanations
Card 7: Final sentence → Closing + Sign-off
```

**Writing Academic Discussion (5-8 cards):**
```
Card 1: Discussion prompt → Position statement
Card 2: Position → First reason
Card 3: First reason → Supporting detail
Card 4: Supporting detail → Second reason/counterargument
Card 5-6: Additional support
Card 7: Final point → Conclusion
```

### Format Rules
- **Stimulus**: Previous sentence OR Question/Situation
- **Response**: Single complete sentence

## 3. Task-Specific Style Requirements

### Speaking Interview
- Tone: Natural, conversational, first-person
- Sentence length: 10-25 words
- Use: Everyday vocabulary, personal examples, direct statements

### Writing Email
- Tone: Match situation formality (formal/semi-formal/friendly)
- Sentence length: 12-20 words
- Use: Appropriate greetings/closings, polite requests, clear purpose statements

### Writing Academic Discussion
- Tone: Academic but conversational (discussion board style)
- Sentence length: 15-30 words
- Use: Formal transitions, logical connectors, hedging language, academic vocabulary

## 4. Output Requirements

### Format
1. **Strictly 2 Columns**: [Stimulus] [TAB] [Response]
2. **NO Header Row**: Start directly with data
3. **NO Code Blocks**: Raw text only
4. **3-10 Cards**: Complete one response chain (varies by task type)

### Quality Checks
- ✓ Each response naturally follows stimulus
- ✓ All sentences are grammatically complete
- ✓ Flow mimics authentic TOEFL response
- ✓ Maintains appropriate tone for task type

## 5. Examples

### Example 1: Speaking Interview (Target 90)
```
Q: Do you prefer studying alone or with friends?	I prefer studying alone because I need a focused environment.
I prefer studying alone because I need a focused environment.	When I study with friends, we tend to get distracted by conversations.
When I study with friends, we tend to get distracted by conversations.	For example, last semester I studied alone for my finals and performed much better.
For example, last semester I studied alone for my finals and performed much better.	That's why I find solo study more effective for me.
```

### Example 2: Writing Email (Target 90)
```
Situation: Request deadline extension from professor for research paper	Dear Professor Johnson, I am writing to request a brief extension for the research paper due on March 15th.
Dear Professor Johnson, I am writing to request a brief extension for the research paper due on March 15th.	I have been working diligently on the assignment, but I recently experienced a family emergency that set me back several days.
I have been working diligently on the assignment, but I recently experienced a family emergency that set me back several days.	I have completed the research and outline, but I need additional time to properly revise and proofread the final draft.
I have completed the research and outline, but I need additional time to properly revise and proofread the final draft.	Would it be possible to submit the paper by March 20th instead?
Would it be possible to submit the paper by March 20th instead?	I understand this is short notice and I apologize for any inconvenience.
I understand this is short notice and I apologize for any inconvenience.	I am committed to submitting high-quality work and would greatly appreciate your consideration.
I am committed to submitting high-quality work and would greatly appreciate your consideration.	Thank you for your understanding.
Thank you for your understanding.	Best regards, Alex Chen
```

### Example 3: Writing Academic Discussion (Target 100+)
```
Prompt: "Some argue that social media has negative impact on society. Student A says it spreads misinformation. Student B says it connects people. Your perspective?"	I appreciate both perspectives, but I believe the impact of social media largely depends on how we use it.
I appreciate both perspectives, but I believe the impact of social media largely depends on how we use it.	While Student A raises a valid concern about misinformation, this problem existed before social media—it simply spreads faster now.
While Student A raises a valid concern about misinformation, this problem existed before social media—it simply spreads faster now.	On the other hand, Student B's point about connection is crucial, especially considering how social media enabled people to maintain relationships during the pandemic.
On the other hand, Student B's point about connection is crucial, especially considering how social media enabled people to maintain relationships during the pandemic.	However, I would add that social media also provides marginalized communities with platforms to share their voices and organize for social change.
However, I would add that social media also provides marginalized communities with platforms to share their voices and organize for social change.	For instance, many successful grassroots movements have originated on social platforms.
For instance, many successful grassroots movements have originated on social platforms.	Therefore, rather than labeling social media as purely positive or negative, we should focus on developing digital literacy skills.
Therefore, rather than labeling social media as purely positive or negative, we should focus on developing digital literacy skills.	This approach allows us to maximize social media's benefits while minimizing its drawbacks.
```

---

**Usage Note**: Generate 5-10 complete response chains per topic for comprehensive coverage. Vary question types and situations within each task type to build adaptability.