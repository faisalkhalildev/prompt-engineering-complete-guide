# Prompt Engineering Complete Guide for Developers

![Prompt Engineering Complete Guide hero](assets/hero-banner.png)

**Prepared By: Senior Software Engineer**

Personalized For: Coder  ·  Daily AI User  ·  Coding & Tech Projects

Version 2.0  ·  Updated April 2025

**Path: Beginner  →  Intermediate  →  Professional**

| 7 Sections | 12 Techniques | 20+ Code Examples | 4 Weeks To Pro Level |
| :---: | :---: | :---: | :---: |

*"A great prompt is not a question — it is a specification."*

— Senior AI Engineering Principle

**Who This Guide Is For**

This guide is for developers, daily AI users, and technical learners who want better results from ChatGPT, coding assistants, and other LLM tools.

**Before You Use This Guide**

- Treat AI output as a draft, not production truth.
- Verify security, correctness, and edge cases before shipping.
- Use the examples in this guide as patterns to adapt, not rigid scripts.

**Table of Contents**

- [Section 1 — What Is Prompt Engineering?](#section-1--what-is-prompt-engineering)
- [Why Does This Matter for Coders?](#why-does-this-matter-for-coders)
- [The 3 Root Causes of Weak Prompts](#the-3-root-causes-of-weak-prompts)
- [Section 2 — The 5-Part Coding Prompt Formula](#section-2--the-5-part-coding-prompt-formula)
- [Full Real Example — Before & After](#full-real-example--before--after)
- [Exercise — Practice the Formula](#exercise--practice-the-formula)
- [Section 3 — Core Techniques (Beginner to Intermediate)](#section-3--core-techniques-beginner-to-intermediate)
- [Technique 1 — Debug Prompts](#technique-1--debug-prompts)
- [Technique 2 — Planning Before Coding](#technique-2--planning-before-coding)
- [Technique 3 — Few-Shot Prompting](#technique-3--few-shot-prompting)
- [Technique 4 — Prompt Chaining](#technique-4--prompt-chaining)
- [Section 4 — Pro-Level Techniques](#section-4--pro-level-techniques)
- [Pro Technique 1 — The System Prompt](#pro-technique-1--the-system-prompt)
- [Pro Technique 2 — The Code Review Prompt](#pro-technique-2--the-code-review-prompt)
- [Pro Technique 3 — Iterative Refinement](#pro-technique-3--iterative-refinement)
- [Pro Technique 4 — A/B Prompt Testing](#pro-technique-4--ab-prompt-testing)
- [Pro Technique 5 — When AI Is Wrong](#pro-technique-5--when-ai-is-wrong)
- [Section 5 — What TO DO and What NOT TO DO](#section-5--what-to-do-and-what-not-to-do)
- [General Prompting Rules](#general-prompting-rules)
- [Coding-Specific Rules](#coding-specific-rules)
- [6 Critical Mistakes That Destroy Results](#6-critical-mistakes-that-destroy-results)
- [Prompt Length Guide — Short vs Long](#prompt-length-guide--short-vs-long)
- [Section 6 — Your 4-Week Learning Plan](#section-6--your-4-week-learning-plan)
- [Daily 30-Minute Practice Routine](#daily-30-minute-practice-routine)
- [How to Build Your Personal Prompt Library](#how-to-build-your-personal-prompt-library)
- [Progress Checklist — Beginner → Professional](#progress-checklist--beginner--professional)
- [Section 7 — Quick Reference Cheat Sheet](#section-7--quick-reference-cheat-sheet)
- [Copy-Paste Phrase Library](#copy-paste-phrase-library)
![Section 1 banner](assets/section-1-banner.png)

# **Section 1 — What Is Prompt Engineering?**

Prompt Engineering is the skill of writing instructions to AI in a precise, structured way so that AI gives you the best, most useful answer. Think of it like being a clear manager: a good manager gives exact instructions, not vague ones.

| 💡 Simple Definition |
| :---- |
| Prompt  \=  The text / question / instruction you give to AI. |
| Engineering  \=  Designing it carefully with structure, context, and rules. |
| Prompt Engineering  \=  Writing prompts that consistently produce clearer, more useful results. |

## **Why Does This Matter for Coders?**

You already use AI every day for coding. But weak prompts give you:

* Generic code that does not match your project or stack

* Wrong bug fixes because AI did not know your environment

* Wasted time fixing bad AI output instead of building

* Missed opportunities — AI can do 10x more than you ask

**With strong prompts you get:**

* Code that matches your exact tech stack and naming style

* Precise bug fixes with explanations you can learn from

* Architecture plans, tests, and documentation in minutes

* AI that can support you like a strong technical partner when you give it enough context

## **The 3 Root Causes of Weak Prompts**

| ❌  WEAK PROMPT | ✅  STRONG PROMPT |
| :---- | :---- |
| fix my code // AI guesses everything // No context at all | You are a senior Node.js developer. Stack: Node 18 \+ Express \+ MongoDB Fix this bug: \[paste code\] Error: TypeError — cannot read property of undefined (line 42\) What I tried: checked middleware ✓ Explain why it failed \+ fix it. |

![Section 2 banner](assets/section-2-banner.png)

# **Section 2 — The 5-Part Coding Prompt Formula**

This is one of the most useful techniques in the entire guide. In practice, this formula improves a large share of weak coding prompts because it adds the missing context AI usually needs.

| 🔑 The Formula |
| :---- |
| PERFECT PROMPT  \=  ROLE  \+  STACK  \+  TASK  \+  RULES  \+  FORMAT |

![Prompt formula visual](assets/formula-visual.png)

| PART | WHAT IT MEANS | EXAMPLE |
| :---- | :---- | :---- |
| **ROLE** | Who should AI be? | You are a senior Python developer... |
| **STACK** | Your tech setup | Python 3.11, FastAPI, PostgreSQL |
| **TASK** | What exactly to do | Write a JWT login function that... |
| **RULES** | Constraints & limits | Use bcrypt. No print(). Handle errors. |
| **FORMAT** | How to output | Code only \+ short inline comments. |

## **Full Real Example — Before & After**

| ❌  WEAK PROMPT | ✅  STRONG PROMPT |
| :---- | :---- |
| write a login function | You are a senior Python developer. Stack: Python 3.11, FastAPI, PostgreSQL Task: Write a user login function that:   \- Accepts email \+ password   \- Checks against DB with SQLAlchemy   \- Returns JWT token on success   \- Returns 401 on wrong credentials Rules: Use bcrypt for password check.   Raise HTTPException for errors.   No print() statements. Format: Clean code \+ short comments. |

## **EXERCISE — Practice the Formula**

| 📝 Your Task |
| :---- |
| Rewrite this weak prompt using the 5-Part Formula: |
|  |
|    "make a button component" |
|  |
| Think about: |
|   → What framework? (React, Vue, Angular?) |
|   → TypeScript or JavaScript? |
|   → What props does the button need? |
|   → What styling system? (Tailwind, CSS modules?) |
|   → Do you want tests included? |
|  |
| Write your improved prompt here: |
|   \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_ |
|   \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_ |
|   \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_ |

| ✅ Model Answer — Sample Strong Prompt |
| :---- |
| You are a senior React developer. |
| Stack: React 18 \+ TypeScript \+ Tailwind CSS |
| Task: Create a reusable Button component with these props: |
|   \- label: string (button text) |
|   \- onClick: () \=\> void |
|   \- variant: "primary" | "secondary" | "danger" |
|   \- disabled?: boolean (optional) |
|   \- isLoading?: boolean (shows spinner when true) |
| Rules: |
|   \- Use TypeScript interface for props |
|   \- Tailwind classes only — no inline styles |
|   \- Export the component as default |
|   \- Handle disabled state visually |
| Format: Component code \+ usage example below it. |

| 💡 Lesson from Model Answer |
| :---- |
| Notice what changed: we went from 3 words to a full specification. |
| The AI now knows: framework, language, styling, props, rules, and format. |
| Result: you get exactly what you need, no manual editing required. |

![Section 3 banner](assets/section-3-banner.png)

# **Section 3 — Core Techniques (Beginner to Intermediate)**

## **Technique 1 — Debug Prompts**

Debugging is where most coders waste the most time with AI. They paste the error and nothing else. Here is the correct template every time:

| 🐛 The Debug Template — Always Use This |
| :---- |
| You are a senior \[language\] developer. |
|  |
| I have a bug. Please help me fix it. |
|  |
| Environment: \[language version, framework, OS if relevant\] |
| Error message: \[paste the FULL error here — every line\] |
|  |
| My code: |
| \`\`\` |
| \[paste only the relevant code — not the whole file\] |
| \`\`\` |
|  |
| What I already tried: |
| \- \[attempt 1\] |
| \- \[attempt 2\] |
|  |
| Question: \[specific question about the bug\] |
|  |
| After fixing: explain in 2 sentences WHY this bug happened |
| so I can avoid it in future projects. |

### **EXERCISE — Write a Debug Prompt**

| 📝 Your Task |
| :---- |
| You have this error in your React app: |
|    TypeError: Cannot read properties of undefined (reading "map") |
|  |
| Write a complete debug prompt using the template above. |
| Include: environment, your code, what you tried. |
|  |
| Your prompt: |
|   \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_ |
|   \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_ |
|   \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_ |
|   \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_ |

| ✅ Model Answer — Debug Prompt for .map() Error |
| :---- |
| You are a senior React developer. |
|  |
| Environment: React 18 \+ JavaScript, Node 18 |
| Error: TypeError: Cannot read properties of |
|        undefined (reading "map") |
|  |
| My code: |
| \`\`\` |
| const UserList \= ({ users }) \=\> { |
|   return ( |
|     \<ul\> |
|       {users.map(user \=\> \<li key={user.id}\>{user.name}\</li\>)} |
|     \</ul\> |
|   ); |
| }; |
| \`\`\` |
|  |
| What I tried: |
| \- Checked that the API call is working ✓ |
| \- Console.log(users) shows undefined on first render |
|  |
| Question: Why is users undefined even though data is fetched? |
|  |
| After fixing: explain in 2 sentences why this happened. |

| ⚠️ Common Mistakes with Debug Prompts |
| :---- |
| Mistake 1: Pasting only the error message — no code |
|            → AI guesses what your code looks like. Often wrong. |
|  |
| Mistake 2: Pasting your entire 200-line file |
|            → AI gets confused. Paste only the relevant function/block. |
|  |
| Mistake 3: Not saying what you already tried |
|            → AI suggests things you already know do not work. |

## **Technique 2 — Planning Before Coding**

For complex coding tasks — system design, algorithms, architecture — it helps to ask AI to plan before it writes code. The goal is not more words; it is better structure.

| 🧠 Magic Phrases — Add to Any Hard Prompt |
| :---- |
| "Plan briefly before writing code." |
| "Plan the architecture first, then write the implementation." |
| "List the edge cases before solving." |
| "Analyze the time complexity first, then optimize." |

| 📌 Planning Example — Algorithm Optimization |
| :---- |
| You are a senior Python engineer. |
|  |
| My function is O(n²) and too slow: |
|  |
| def find\_duplicates(arr): |
|     result \= \[\] |
|     for i in range(len(arr)): |
|         for j in range(i+1, len(arr)): |
|             if arr\[i\] \== arr\[j\]: |
|                 result.append(arr\[i\]) |
|     return result |
|  |
| Think step by step: |
|   1\. What is the bottleneck? |
|   2\. What data structure can optimize this? |
|   3\. What is the best possible time complexity? |
| Then rewrite it with an explanation of each change. |

| ⚠️ Common Mistake with Planning Prompts |
| :---- |
| Wrong:  "Think step by step and fix my code." |
|          → Too vague. AI writes text and still skips planning. |
|  |
| Right:  "Before writing any code, list: (1) the components needed, |
|          (2) the data flow, (3) the edge cases. Then code." |
|          → You give AI a structured plan to follow. |

## **Technique 3 — Few-Shot Prompting**

Want AI to write code that exactly matches YOUR style? Show it 1-2 examples of your existing code. AI will instantly learn your patterns, naming conventions, and structure.

| 📚 Few-Shot Example — Teaching Your API Style |
| :---- |
| Here is how I write my API routes. Follow this exact pattern: |
|  |
| // My style: |
| router.get("/users", authenticate, async (req, res) \=\> { |
|   try { |
|     const users \= await User.findAll(); |
|     res.json({ success: true, data: users }); |
|   } catch (err) { |
|     res.status(500).json({ success: false, error: err.message }); |
|   } |
| }); |
|  |
| Now write a POST /products route using the EXACT same |
| structure, error handling style, and response format. |
| Stack: Express 4 \+ Sequelize ORM \+ PostgreSQL. |

| ⚠️ Common Mistake with Few-Shot |
| :---- |
| Mistake: Showing AI your example but not saying "follow this pattern" |
|           → AI sees your example as context only — not as a rule. |
|  |
| Fix: Always end with: "Follow this exact pattern / naming convention. |
|      Do not change the structure." |

## **Technique 4 — Prompt Chaining**

Never ask AI to build a large feature in one single prompt. Break it into a chain. Each prompt uses the output from the previous one. Here is a fully written-out real example:

| 🔗 Full Example — Building a User Auth System |
| :---- |
| ━━ PROMPT 1 — Architecture (paste this first) ━━ |
|  |
| "You are a senior backend architect. |
|  Plan the architecture for a JWT user authentication system. |
|  List all files, components, and data flow. |
|  Stack: Node.js 18 \+ Express \+ PostgreSQL \+ Prisma. |
|  No code yet — only the plan." |
|  |
| ━━ PROMPT 2 — Database (after you get the plan) ━━ |
|  |
| "Using that architecture plan, write the Prisma schema. |
|  Include: User model with id, email, password, createdAt. |
|  Add the migration command to run after." |
|  |
| ━━ PROMPT 3 — Core Logic (after schema) ━━ |
|  |
| "Now write the auth service (auth.service.js). |
|  Functions: register(email, password) and login(email, password). |
|  Use bcrypt for hashing. Return JWT on login. |
|  Use the Prisma schema from above." |
|  |
| ━━ PROMPT 4 — Tests (after service) ━━ |
|  |
| "Write Jest unit tests for the auth service. |
|  Cover: successful register, duplicate email error, |
|  successful login, wrong password error." |
|  |
| ━━ PROMPT 5 — Documentation (after tests) ━━ |
|  |
| "Write the OpenAPI/Swagger YAML documentation |
|  for POST /auth/register and POST /auth/login." |

| ⚠️ Common Mistake with Prompt Chaining |
| :---- |
| Mistake: Starting Step 3 without confirming Step 2 output is correct. |
|           → Errors compound — wrong schema leads to wrong service code. |
|  |
| Rule: Always review AI output before moving to the next step. |
|       If Step 2 is 80% right, fix it first. Then proceed. |

![Section 4 banner](assets/section-4-banner.png)

# **Section 4 — Pro-Level Techniques**

These techniques are used by engineers who build real AI-powered products. They separate AI users from AI engineers.

## **Pro Technique 1 — The System Prompt**

A system prompt is a permanent set of rules and context you give AI at the start of every conversation. This is how you build AI assistants that always know your project.

| ⚙️ System Prompt Template (blank) |
| :---- |
| You are a senior developer working on MY project. |
|  |
| Project: \[your project name and description\] |
| Stack: \[e.g. React 18 \+ TypeScript \+ Node.js \+ PostgreSQL\] |
| Styling: \[e.g. Tailwind CSS\] |
| Testing: \[e.g. Jest \+ React Testing Library\] |
| State: \[e.g. Zustand / Redux\] |
|  |
| Code style rules: |
| \- Functional components only. No class components. |
| \- Always add TypeScript types to everything. |
| \- Use async/await. Never use .then() chaining. |
| \- Add JSDoc comments to all exported functions. |
| \- Files: kebab-case. Functions: camelCase. Types: PascalCase. |
|  |
| Always follow these rules in every answer. |
| When unsure about something in my project, ask before assuming. |

| ✅ Real Filled Example — E-Commerce Project |
| :---- |
| You are a senior developer working on MY project. |
|  |
| Project: ShopEasy — an e-commerce web app for handmade jewelry. |
| Stack: React 18 \+ TypeScript \+ Node.js 18 \+ PostgreSQL 15 |
| ORM: Prisma |
| Styling: Tailwind CSS v3 |
| Testing: Jest \+ React Testing Library \+ Supertest |
| State: Zustand |
| Auth: JWT with refresh tokens |
|  |
| Code style rules: |
| \- Functional components only. No class components. |
| \- Always add TypeScript interfaces — never use "any". |
| \- Use async/await. Never use .then() chaining. |
| \- Error responses: { success: false, error: string } |
| \- Success responses: { success: true, data: T } |
| \- File names: kebab-case (user-service.ts) |
| \- Function names: camelCase (getUserById) |
| \- Type names: PascalCase (UserWithOrders) |
|  |
| Always follow these rules in every answer. |

| 💡 How to Use Your System Prompt |
| :---- |
| Step 1: Save it in a text file called "my-project-prompt.txt" |
| Step 2: At the START of every new chat, paste it in first. |
| Step 3: Then ask your coding question normally. |
| Step 4: AI remembers your entire stack for the whole session. |
| Step 5: When your project changes, update the file and bump version. |

## **Pro Technique 2 — The Code Review Prompt**

| 🔍 Code Review Template |
| :---- |
| Act as a senior software engineer doing a formal code review. |
|  |
| Review this code for: |
|   1\. Bugs or logic errors |
|   2\. Security vulnerabilities (injection, auth issues, exposed secrets) |
|   3\. Performance problems (N+1 queries, memory leaks, O(n²)) |
|   4\. Code readability and maintainability |
|   5\. Missing error handling |
|   6\. SOLID / DRY / KISS violations |
|  |
| // My code: |
| \[paste your code here\] |
|  |
| For each issue found: |
|   \- Location: \[line number or function name\] |
|   \- Problem: \[what is wrong\] |
|   \- Fix: \[exact corrected code\] |
|   \- Severity: \[HIGH / MEDIUM / LOW\] |
|  |
| End with: overall score /10 \+ one top improvement tip. |

## **Pro Technique 3 — Iterative Refinement**

Professionals rarely accept the first answer as final. They iterate, verify, and refine until the output fits the real task.

| 🔁 Refinement Rounds — Real Workflow |
| :---- |
| Round 1:  Get the initial code |
|  |
| Round 2:  "Now add full TypeScript types to every |
|            function parameter and return value." |
|  |
| Round 3:  "Refactor to async/await. Remove all .then() chains. |
|            Keep the exact same logic." |
|  |
| Round 4:  "Optimize for performance. |
|            What is the current time complexity? |
|            Can it be improved? Show before \+ after." |
|  |
| Round 5:  "Write JSDoc comments for every exported |
|            function. Include @param and @returns." |
|  |
| Round 6:  "Write unit tests for the 3 main edge cases." |

## **Pro Technique 4 — A/B Prompt Testing**

Write 2 different versions of the same prompt and compare results. This is how professionals find the BEST prompt. Then save the winner in your library.

| 🔬 A/B Testing — Step by Step |
| :---- |
| Step 1:  Write Prompt A (your current way) |
| Step 2:  Write Prompt B (improved version using formula) |
| Step 3:  Send BOTH to AI. Compare answers. |
| Step 4:  Rate each on: accuracy, completeness, code quality. |
| Step 5:  Save the winner in your prompt library. |
| Step 6:  Next week, try to beat the winner with Prompt C. |
|  |
| Example: |
|   A:  "write an API rate limiter" |
|   B:  "You are a senior Node.js engineer. Stack: Express 4\. |
|        Write a rate limiter middleware: max 100 req/15min |
|        per IP. Use express-rate-limit. Add JSDoc comments. |
|        Show usage example at the bottom." |
|   Result: B wins every time. Save B. Done. |

## **Pro Technique 5 — When AI Is Wrong**

Beginners give up when AI is wrong. Professionals know how to correct AI and guide it back on track. Here are the 3 steps:

| 🛑 When AI Gives a Wrong Answer — 3 Steps |
| :---- |
| Step 1 — Tell AI it is wrong and exactly WHY: |
|   "This is incorrect. The issue is that you used .findOne() |
|    but my Prisma version requires .findUnique()." |
|  |
| Step 2 — Give AI the correct information: |
|   "The correct Prisma method is findUnique({ where: { id } }). |
|    Here is the Prisma docs reference: \[paste relevant snippet\]" |
|  |
| Step 3 — Ask it to try again with the correction: |
|   "Please rewrite the function using findUnique.", |
|    Keep all other logic the same." |
|  |
| IMPORTANT: Never say only "this is wrong — try again". |
| AI needs to know WHAT is wrong and WHY. |

![Section 5 banner](assets/section-5-banner.png)

# **Section 5 — What TO DO and What NOT TO DO**

These rules are the clearest in the guide. Follow the green column. Avoid the red column. Every rule here comes from real mistakes engineers make daily.

## **General Prompting Rules**

| ✅  DO THIS | ❌  NEVER DO THIS |
| :---- | :---- |
| ✓  Always give AI a role: 'You are a senior...' | ✗  Start with just the question — no context at all |
| ✓  Include your tech stack in every coding prompt | ✗  Expect AI to guess your language or framework |
| ✓  Be specific: length, format, language, style, version | ✗  Use vague words like 'good', 'proper', 'nice', 'better' |
| ✓  Iterate and refine after every response | ✗  Accept the first answer and give up if it is not perfect |
| ✓  Tell AI what NOT to do (negative instructions) | ✗  Only say what you want and hope AI avoids bad habits |
| ✓  Break big tasks into small chains of prompts | ✗  Ask for an entire complex feature in one single prompt |
| ✓  Save your best prompts in a personal library | ✗  Rewrite the same prompt from scratch every time |

## **Coding-Specific Rules**

| ✅  DO THIS | ❌  NEVER DO THIS |
| :---- | :---- |
| ✓  Paste the FULL error message including the entire stack trace | ✗  Write the error from memory or paste only the first line |
| ✓  Show AI 1-2 examples of your code style first | ✗  Let AI choose its own naming and structure conventions |
| ✓  Ask AI to explain the bug — not just fix it | ✗  Just copy-paste the fix without understanding why it failed |
| ✓  Ask for code \+ tests \+ documentation together | ✗  Forget tests and docs until the very end of the project |
| ✓  Ask for time/space complexity on algorithm tasks | ✗  Accept code without knowing if it is efficient or scalable |
| ✓  Ask AI to plan first on architecture tasks | ✗  Get a direct answer that skips planning and trade-offs |
| ✓  Tell AI the wrong answer and why when it makes mistakes | ✗  Just say 'this is wrong, try again' with no explanation |

## **6 Critical Mistakes That Destroy Results**

| ⚠️ Diagnose Yourself — Which of These Do You Still Do? |
| :---- |
| Mistake 1: Vague task — "fix this" / "improve this" / "make it better" |
|            → AI does not know what "fix" or "better" means. |
|            Fix: Be specific — "fix the null check on line 12" |
|  |
| Mistake 2: No stack — AI generates code for the wrong framework |
|            → You waste time adapting generic code to your project. |
|            Fix: Always say language \+ framework \+ version |
|  |
| Mistake 3: Too much at once — "build my entire authentication system" |
|            → AI gives shallow, incomplete answer for everything. |
|            Fix: Break into 5 chained prompts (see Section 3\) |
|  |
| Mistake 4: Ignoring first response without giving feedback |
|            → The answer may be 80% right — you just need to refine. |
|            Fix: Iterate with specific refinement instructions |
|  |
| Mistake 5: Not saving good prompts — rewriting every time |
|            → Wasted effort repeating work you already did. |
|            Fix: Build a prompt library — save every winner |
|  |
| Mistake 6: Trusting AI code without testing it |
|            → Always run and test AI code before using in production. |
|            Fix: Add "write tests for this" to every code prompt |

## **Prompt Length Guide — Short vs Long**

| TASK TYPE | PROMPT LENGTH | REASON |
| :---- | :---- | :---- |
| **Quick fix / rename variable** | **1-3 lines** | Simple task, AI needs very little context |
| **Bug fix** | **5-10 lines** | Needs error \+ code \+ environment |
| **Single function / component** | **8-15 lines** | Needs role \+ stack \+ task \+ rules \+ format |
| **Full feature** | **15-25 lines per step** | Use chaining — one detailed prompt per step |
| **System design / architecture** | **20-30 lines** | Needs planning — ask AI to outline the approach before coding |

![Section 6 banner](assets/section-6-banner.png)

# **Section 6 — Your 4-Week Learning Plan**

Prompt Engineering is a skill like any other. You build it by practicing daily. Here is your exact plan — 30 minutes per day, measurable goals every week.

![Progress tracker](assets/section-7-banner.png)

| WEEK | FOCUS | DAILY PRACTICE (30 min) | MEASURABLE GOAL |
| :---- | :---- | :---- | :---- |
| **Week 1** | **Foundation** | Use 5-part formula for every prompt. Rewrite 3 old weak prompts daily. Save best prompts in a file. | Zero vague prompts. Always include Role \+ Stack \+ Task. |
| **Week 2** | **Debug + Planning** | Use the debug template for every bug. Ask AI to outline the approach on harder tasks. Ask AI to explain every bug. | Fix bugs faster and get clearer explanations for why they happened. |
| **Week 3** | **Chain \+ Style** | Build 1 full feature using 5-step chain. Show AI 2 code examples before each request. | Full features built with AI. AI matches your exact coding style. |
| **Week 4** | **Pro Level** | Create your project system prompt. Do AI code reviews daily. A/B test 3 prompt pairs. | Build a complete CRUD API draft with plan, code, tests, and docs, then review and validate it yourself. |

## **Daily 30-Minute Practice Routine**

| 📅 Every Day — 3 Steps |
| :---- |
| 1\. WARM UP (5 min) |
|    Open your prompt library. Read 2-3 saved prompts. |
|    Ask: how can I improve one of them today? |
|  |
| 2\. PRACTICE (20 min) |
|    Use AI for your real work — but consciously. |
|    For every prompt: use the formula. Iterate at least twice. |
|    If you get a bad answer — do not give up. Refine it. |
|    If AI is wrong — use the 3-step correction technique. |
|  |
| 3\. REVIEW (5 min) |
|    Save your 1 best prompt of the day in your library. |
|    Write one note: what made this prompt work well? |

## **How to Build Your Personal Prompt Library**

Your prompt library is your most valuable asset. It is a collection of your best, tested, reusable prompts. Start it today.

* **Tool:** Use Notion, Google Docs, VS Code snippets, or a plain text file

* **Categories:** Debug / Code Gen / Code Review / Architecture / Tests / Docs

* **For each prompt save:** The prompt \+ what task it solves \+ why it works \+ date added

* **Version it:** When you improve a prompt, keep the old version. Compare over time.

* **Goal:** Have 20+ saved prompts by end of Week 4

## **Progress Checklist — Beginner → Professional**

| 📊 Check Your Level |
| :---- |
| BEGINNER (End of Week 1-2) — you should be able to: |
|   ✓ Write every prompt with Role \+ Stack \+ Task \+ Rules \+ Format |
|   ✓ Never write vague prompts ("fix this", "make it better") |
|   ✓ Write debug prompts with full error \+ code \+ what you tried |
|   ✓ Ask AI to explain every bug — not just fix it |
|  |
| INTERMEDIATE (End of Week 3\) — you should be able to: |
|   ✓ Ask AI to plan first on architecture or algorithm tasks |
|   ✓ Show AI your code style with 2 examples before each request |
|   ✓ Build full features using 5-step chained prompts |
|   ✓ Iterate every AI response at least 2-3 times |
|   ✓ Correct AI when it is wrong using the 3-step method |
|  |
| PROFESSIONAL (End of Week 4+) — you should be able to: |
|   ✓ Have a system prompt ready for every project |
|   ✓ Run AI code reviews before every pull request |
|   ✓ A/B test prompts and always keep the best version |
|   ✓ Have 20+ tested, reusable prompts saved in your library |
|   ✓ Build a complete CRUD API draft (plan + code + tests + docs) and validate it before shipping |
|   ✓ Help other developers improve their prompts |

![Section 7 banner](assets/section-7-cheat-sheet.png)

# **Section 7 — Quick Reference Cheat Sheet**

![Footer banner](assets/footer-banner.png)

## **Copy-Paste Phrase Library**

| GOAL | PHRASE TO ADD |
| :---- | :---- |
| **Force thinking** | "Plan briefly before writing code." |
| **Force planning** | "Plan the architecture first. No code yet." |
| **Match my style** | "Here is my code style. Follow it exactly: \[example\]" |
| **Understand bug** | "After fixing, explain WHY this happened in 2 sentences." |
| **Control length** | "Keep your answer under 50 lines. Be concise." |
| **Get alternatives** | "Give me 3 different approaches. I will choose one." |
| **Refine output** | "Now make it more efficient / add TypeScript / add error handling." |
| **Code review** | "Review for bugs, security, performance. Rate each: HIGH/MEDIUM/LOW." |
| **No bad habits** | "Do NOT use class components. Do NOT use var. No console.log()." |
| **Multiple options** | "For each: show code, explain trade-off, rate complexity 1-5." |
| **Correct AI** | "This is wrong because \[reason\]. The correct way is \[info\]. Try again." |
| **Add tests** | "Now write Jest unit tests for the 3 main edge cases of this function." |

*"Every expert was once a beginner. The difference is they started and did not stop."*

**Open Section 2\. Do the exercise. That is your first task. Start now.**













