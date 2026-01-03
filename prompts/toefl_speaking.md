# Anki TSV Generator: 2026 TOEFL Speaking/Writing (Full Response Mode)

Generate complete question-answer pairs for TOEFL practice.
Each card contains: **[Question]** → **[Complete Answer]**

## 1. Configuration (Select One)

### Task Type
- **Speaking Interview** (45 sec, 3-4 sentences, 50-70 words, conversational tone)
- **Writing Email** (7 min, 6-10 sentences, 100-150 words, appropriate formality)
- **Writing Academic Discussion** (10 min, 5-8 sentences, 100-150 words, academic tone)

### Difficulty Level
- **Target 80** (Simple vocabulary, basic structure, clear and direct)
- **Target 90** (Academic vocabulary, varied structure, natural flow)
- **Target 100+** (Sophisticated expressions, complex syntax, nuanced arguments)

### Topic Selection
Use common TOEFL topics across academic and daily life contexts.

## 2. TSV Format Structure (Strict)

**Fields:** Question | Answer

### Format Rules
- **Question**: Single question or situation prompt
- **Answer**: Complete response (full sentences, appropriate length for task type)
- **NO intermediate steps**: One card = one complete response

## 3. Task-Specific Guidelines

### Speaking Interview
- Length: 3-4 sentences, 50-70 words total
- Structure: Opinion/Answer → Reason/Detail → Example (optional) → Conclusion (optional)
- Tone: Natural, conversational, first-person
- Delivery: Can be spoken smoothly in 20-30 seconds (leaving buffer time)

### Writing Email
- Length: 6-10 sentences, 100-150 words
- Structure: Greeting → Purpose → Main content (2-4 sentences) → Closing action → Sign-off
- Tone: Match situation (formal/semi-formal/friendly)
- Include: Proper email format with subject line when appropriate

### Writing Academic Discussion
- Length: 5-8 sentences, 100-150 words
- Structure: Position → Reason 1 + support → Reason 2 + support (or counterargument) → Conclusion
- Tone: Academic but conversational (discussion board style)
- Style: Use transitions, logical flow, reference discussion topic naturally

## 4. Output Requirements

### Format
1. **Strictly 2 Columns**: [Question] [TAB] [Answer]
2. **NO Header Row**: Start directly with data
3. **NO Code Blocks**: Raw text only
4. **10-15 Cards**: Complete set for one practice session

### Quality Checks
- ✓ Each answer is complete and self-contained
- ✓ Length matches task type requirements
- ✓ Tone is appropriate for task type
- ✓ Natural English that can be memorized and reproduced
- ✓ Answers demonstrate variety (different structures, expressions)

## 5. Examples

### Example 1: Speaking Interview (Target 90)
```
Do you prefer studying alone or with friends?	I prefer studying alone because I need a focused environment. When I study with friends, we tend to get distracted by conversations. For example, last semester I studied alone for my finals and performed much better. That's why I find solo study more effective for me.
What do you think about online learning?	I believe online learning offers great flexibility for students. It allows people to study at their own pace and access courses from anywhere. However, I think it requires strong self-discipline to stay motivated. Overall, I see it as a valuable option alongside traditional education.
How important is physical exercise for students?	I think regular exercise is essential for students' wellbeing. It helps reduce stress from academic pressure and improves concentration in class. Personally, I notice I can focus better after going for a run. So I'd say it should be part of every student's routine.
```

### Example 2: Writing Email (Target 90)
```
You need to request a deadline extension from your professor for a research paper. Write an email.	Subject: Request for Extension on Research Paper\n\nDear Professor Johnson,\n\nI am writing to request a brief extension for the research paper due on March 15th. I have been working diligently on the assignment, but I recently experienced a family emergency that set me back several days.\n\nI have completed the research and outline, but I need additional time to properly revise and proofread the final draft. Would it be possible to submit the paper by March 20th instead?\n\nI understand this is short notice and I apologize for any inconvenience. I am committed to submitting high-quality work and would greatly appreciate your consideration.\n\nThank you for your understanding.\n\nBest regards,\nAlex Chen
You ordered a product online but received the wrong item. Write an email to customer service.	Subject: Wrong Item Received - Order #84521\n\nDear Customer Service Team,\n\nI am writing regarding order #84521 placed on February 10th. I ordered a blue wireless keyboard, but I received a black wireless mouse instead.\n\nThe package arrived yesterday in good condition, but the contents do not match my order. I have attached a photo of the item I received and a copy of my order confirmation.\n\nCould you please arrange to send me the correct item? I would also like to know the procedure for returning the wrong product.\n\nI would appreciate a prompt response as I need the keyboard for work. Thank you for your assistance in resolving this matter.\n\nSincerely,\nSarah Williams
Your roommate is being too noisy late at night. Write a friendly email addressing this issue.	Subject: Quick Chat About Evening Noise\n\nHi Jordan,\n\nHope you're doing well! I wanted to reach out about something that's been on my mind lately.\n\nI've noticed that there's been quite a bit of noise coming from your room late at night, especially after 11 PM. I have early morning classes and I'm finding it difficult to get enough sleep on weeknights.\n\nI completely understand that you have a different schedule, and I'm not trying to be difficult. Would it be possible to keep the volume down after 11 on weeknights? I'm happy to discuss a compromise that works for both of us.\n\nLet me know when you're free to chat about this. Thanks for understanding!\n\nBest,\nTaylor
```

### Example 3: Writing Academic Discussion (Target 100+)
```
Professor: "Some argue that social media has a negative impact on society, while others believe it brings people together. What is your perspective?"\n\nStudent A: "I think social media does more harm than good because it spreads misinformation quickly."\n\nStudent B: "I disagree. Social media helps people stay connected across distances."	I appreciate both perspectives, but I believe the impact of social media largely depends on how we use it. While Student A raises a valid concern about misinformation, this problem existed before social media—it simply spreads faster now. On the other hand, Student B's point about connection is crucial, especially considering how social media enabled people to maintain relationships during the pandemic. However, I would add that social media also provides marginalized communities with platforms to share their voices and organize for social change. For instance, many successful grassroots movements have originated on social platforms. Therefore, rather than labeling social media as purely positive or negative, we should focus on developing digital literacy skills to maximize its benefits while minimizing its drawbacks.
Professor: "Is it better for companies to prioritize profit or social responsibility?"\n\nStudent A: "Companies should focus on profit because that's how they survive and create jobs."\n\nStudent B: "I think social responsibility is more important because businesses have an obligation to society."	I understand both arguments, but I don't think profit and social responsibility need to be mutually exclusive. Student A correctly points out that profitability ensures business sustainability, which is essential for long-term job creation and economic stability. However, I'd argue that social responsibility can actually enhance profitability rather than detract from it. Research has shown that consumers increasingly prefer brands that demonstrate ethical practices and environmental consciousness. For example, companies like Patagonia have built strong customer loyalty precisely because they prioritize sustainability alongside profits. Furthermore, socially responsible practices often lead to better employee retention and productivity, which ultimately benefits the bottom line. Therefore, I believe the most successful approach is integrating social responsibility into the core business strategy rather than treating it as separate from profit generation.
```

---

**Usage Note**: Generate 10-15 cards per task type. Mix difficulty levels and topics to build comprehensive practice material. Each card should be memorizable as a complete unit that can be reproduced naturally in test conditions.