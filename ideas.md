# 英単語4択テスト — Design Ideas

## Approach 1
- **Theme Name**: 紙面の余白
- **Very Brief Intro**: 学習ノートのような白い余白と細い罫線で、集中と安心感をつくる。毎日の復習に自然になじむ静かな方向性。
- **Probability**: 0.04

## Approach 2
- **Theme Name**: 朱印スタディ
- **Very Brief Intro**: 和紙のニュートラルカラーに朱色のアクセントを重ね、英単語学習を小さな道場のように見せる。短い学習セッションの達成感を視覚化する方向性。
- **Probability**: 0.03

## Approach 3
- **Theme Name**: アーカイブ・ボード
- **Very Brief Intro**: 静かなダークネイビーとオレンジのグロウで、学習ログを編集室のダッシュボードのように扱う。日々の進捗を少しだけゲーム的に感じさせる方向性。
- **Probability**: 0.02

## Chosen Approach: 朱印スタディ

### Design Movement
Japanese editorial stationery meets contemporary learning tool. The visual language borrows from washi paper, library index cards, and a single vermilion seal used as a deliberate focus marker.

### Core Principles
1. **Focus by restraint** — one question, one clear action, and only the supporting metadata needed for the next decision.
2. **Editorial hierarchy** — Japanese labels, English headwords, and answer choices use distinct typographic roles rather than uniform cards.
3. **Warm utility** — surfaces feel tactile and human, while controls remain crisp and fast.
4. **Progress as a ritual** — each completed question leaves a small, legible trace in the session progress.

### Color Philosophy
A warm bone paper background (#F7F3EC) gives the app the calm of a study sheet. Ink navy (#152238) carries primary text and structure; vermilion (#E45A3B) is the ownable signature color and marks active choices, correct answers, and completion. Faded indigo (#6F86A6) supports metadata without competing with the quiz. The palette is intentionally low-saturation except for vermilion, so feedback feels precise rather than alarming.

### Layout Paradigm
An asymmetrical editorial frame: a slim left rail carries the app mark and session context on desktop, while the main content uses a wide reading column and an offset utility column. On mobile the rail becomes a compact masthead, and the question panel fills the viewport with sticky progress context.

### Signature Elements
- A vermilion seal mark made from a square bracket and dot, used as the app logo and on the active answer state.
- Index-card answer options with a small letter tab rather than generic rounded buttons.
- Fine dotted registration marks and a subtle paper grain behind the mode selection screen.

### Interaction Philosophy
The interface answers immediately, like a flashcard flipped on a desk. Options remain calm before selection; after selection, a vermilion rule and concise Japanese feedback make the result obvious. Keyboard keys A–D mirror the printed answer tabs. There is no confirmation step between questions.

### Animation
Use small, physical-feeling transitions only: question content enters with a 180ms upward fade, answer cards lift 2px on hover, and the progress bar fills with a 220ms ease-out. Feedback appears through opacity and transform, never layout jumps. Respect reduced-motion preferences by disabling entrance movement and keeping state changes instant.

### Typography System
- **Display / English headword**: Fraunces 700 for the active word and large numeric score; its editorial serif gives the vocabulary room to breathe.
- **UI / Japanese body**: Zen Kaku Gothic New 400–700 for labels, controls, and explanations; clean kana shapes keep dense quiz content readable.
- **Hierarchy**: eyebrow labels at 11px uppercase tracking, page titles at 32–46px, question headword at clamp(38px, 7vw, 72px), answer labels at 15–17px.

### Brand Essence
A focused four-choice vocabulary drill for learners who want a calm, repeatable way to turn a 2,479-word list into daily progress. **Precise, warm, quietly motivating.**

### Brand Voice
Headlines are short and editorial. CTAs are direct verbs with a little human warmth. Microcopy tells the learner what just happened, never what they should feel.

Example lines:
- “今日の100語を、ひとつずつ。”
- “正解を積む。迷いは次でほどく。”

### Wordmark & Logo
The mark is a bold vermilion square seal containing a navy offset dot and a short open bracket, suggesting an index card corner and a target. The wordmark is set separately in a serif display face as “VOCAB / 4”, never as a default browser wordmark.

### Signature Brand Color
**Vermilion seal — #E45A3B.** It is warm enough to feel human, distinct enough to guide attention, and restrained enough to remain usable for both correct feedback and primary actions.

## Style Decisions
- Keep the UI light, warm, and editorial; do not drift into generic SaaS purple, glassmorphism, or neon gaming motifs.
- Treat every quiz state as a paper index card with a strong typographic hierarchy and a visible answer letter.
- Use generated visuals only for atmospheric surfaces; never place essential question text inside an image.

- **User override**: The app should be surprisingly simple. Remove decorative hero imagery, rail navigation, texture, and heavy shadows; keep only a small seal mark, clear typography, thin rules, and functional cards.
