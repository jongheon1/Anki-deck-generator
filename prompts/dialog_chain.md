# Anki TSV Generator: Dialogue Chain Mode (All-in-One)

This template generates realistic, multi-turn dialogue chains for **Developer & Daily Life** situations.
It breaks down a conversation into "Stimulus (Front)" and "Response (Back)" Anki cards.

## 1. Contexts (Choose One)

### A. Exchange Student & Campus Life
- **Dorm Life**: Resolving roommate conflicts (cleaning, noise), rules.
- **Team Projects**: Assigning roles, handling free riders, discussion.
- **Academic**: Asking professors for extensions, borrowing notes, admin requests.

### B. Global Tech Company & Developer
- **Engineering**: Code review defense, Stand-up updates, Incident response.
- **Communication**: Negotiating deadlines with PM, Salary negotiation, Exit interview.
- **Office Life**: Small talk with colleagues, Mentoring juniors.

### C. Job Interview (Process)
- **Behavioral**: Self-intro, Weaknesses, Conflict resolution (STAR method).
- **Technical**: System design discussion, Explaining thought process in live coding.
- **Closing**: Asking insightful questions to the interviewer.

### D. Real Survival & Travel
- **Service**: Complex ordering (Cafe/Subway), Handling complaints/refunds.
- **Vital Needs**: Explaining symptoms (Hospital/Pharmacy), Haircut requests.
- **Emergency**: Lost & Found, Police, Navigation help.

### E. Social & Dating
- **Making Friends**: Ice breaking at parties, Finding common interests.
- **Romance**: Asking someone out, Flirting, Polite rejection.
- **Deep Talk**: Consoling a friend, Apologizing, Giving compliments.

## 2. Chain Logic (The Flow)

Generate a dialogue of **4-8 turns**. Then split it strictly into pairs:

- **Card 1**: `(Context: Start)` -> `[Person A's line]`
- **Card 2**: `[Person A's line]` -> `[Person B's reply]`
- **Card 3**: `[Person B's reply] + (Hint: What does A ask next?)` -> `[Person A's reply]`
- **Card 4**: `[Person A's reply] + (Hint: How does B respond?)` -> `[Person B's reply]`

*Note: Person B represents the User.*

## 3. TSV Format Structure (Strict)

**Fields:** Stimulus | Response

1. **Stimulus (Front)**: Previous line + **(Context/Intent Hint)**
2. **Response (Back)**: The natural English response.

**Example (Code Review Defense):**
(Context: PR Review, Senior questions library choice)	Why did you use this heavy library for a simple task?
Why did you use... (Explain: Performance trade-off)	I considered that, but we need the caching feature this library provides for scalability.
I considered that... (Senior agrees but worries about size)	Fair point, but I'm worried about the bundle size increasing.
Fair point... (Propose: Tree-shaking solution)	I can configure tree-shaking to only include the modules we need.

## 4. Output Requirements

1. **Strictly 2 Columns**: [Stimulus] [TAB] [Response]
2. **No Headers**: Do not include "Stimulus | Response".
3. **No Code Blocks**: Just raw text lines.
4. **Natural Spoken English**: Use appropriate tone (Formal/Casual/Slang).

## 5. Prompt Template to use

"Create a [LENGTH] dialogue chain about [SPECIFIC CONTEXT].
Role: Person B is the [USER].
Tone: [TONE].
Format: Stimulus [TAB] Response."