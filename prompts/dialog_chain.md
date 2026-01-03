# Anki TSV Generator: Dialogue Chain Mode (All-in-One)

This template generates realistic, multi-turn dialogue chains for **Developer & Daily Life** situations.
It breaks down a conversation into "Stimulus (Front)" and "Response (Back)" Anki cards.

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
