# Collaborating With AI at Work
## A Reference Guide to the QAMH AI Training Series
### TaiLORED IDEAS · Dr Ryan Jesson

---

*This document synthesises the core ideas, frameworks, and lessons from all four sessions of the QAMH AI Training Series. It's designed as a reference you can return to — a distillation of what matters most, in a format that retains the ideas in the way they were actually taught.*

---

## Session 1: The Why
### Building a Foundation for Working with AI as a Thinking Partner

---

### What Are We Actually Dealing With?

When we talk about AI in these sessions, we're talking about one specific type: **large language models** (LLMs). These are the systems behind ChatGPT, Claude, and Gemini.

Here's what they actually do. Rather than storing facts in a database, an LLM has been trained on vast amounts of text — roughly **300 billion words**, or about **2,283 years of reading** if a human tried to get through it all. Through that training, the model has learned the statistical patterns of how language works: how words relate to each other, how sentences are structured, how ideas connect across different domains.

When you send it a message, what it's doing — at a fundamental level — is using everything it knows about language to predict what comes next. That might sound simple. It isn't.

Here's why: **language is not just communication**. Language is the medium through which we form ideas, write knowledge down, reason through problems, construct arguments, and teach each other things. When a system has mapped out how language works at that scale, what emerges looks very much like reasoning, creativity, and understanding — whether or not it's "really" doing those things in the way humans do.

---

### The Bat-and-Ball Problem

A bat and a ball together cost $1.10. The bat costs $1.00 more than the ball. How much does the ball cost?

Most people immediately think: 10 cents.

The answer is 5 cents. (If the ball costs 10 cents and the bat costs $1.00 more, that's $1.10 — which totals $1.20, not $1.10.)

The answer just came to you, fluently and confidently. You didn't effortfully work through it — it felt automatic. That's pattern prediction in action: you have extensive experience with simple subtraction problems, so your brain extrapolated. And got it wrong.

This is the same mechanism that drives LLMs — and it explains both their power and their limitations.

**Hallucinations** are not glitches. They're what happens when the model extrapolates from its experience and lands on something plausible but incorrect. It's not lying; it's doing the same thing you did with the bat-and-ball — pattern-matching at speed, confidently. The hallucination rate has dropped dramatically over the last few years, and good prompting reduces it further. But it's why **human oversight is always essential**.

**Bias** exists because the model has learned from everything humans have written — including our biases, our blind spots, and our errors. It reflects our language back at us, including the patterns we'd rather not see. This is a known limitation with known mitigations, and the field is actively working on it.

The important thing to understand is that **the same mechanism that produces errors is the same mechanism that produces capability**. The flexibility, creativity, and cross-domain reasoning that makes these tools so powerful comes from the same place as the hallucination risk. That's not a contradiction — it's the nature of the system.

---

### Why Should We Use AI at Work?

The research is clear:

- **Speed:** People using LLMs complete tasks in roughly half the time of those who don't.
- **Quality:** Work produced with AI assistance is consistently rated as higher quality by independent judges who don't know which group used AI.
- **Creativity:** Solutions produced with AI assistance are rated as more creative, more viable, and more feasible than those produced without.

But that's the business case. Here's the real reason:

Two years ago, statistics was a dark and scary place. Not something abstract — genuinely frightening, the kind of thing that made starting a PhD day feel overwhelming. Then ChatGPT arrived, and what followed was a series of conversations: *Hey mate, I've done this experiment. Here's the data. What's the best way to analyse this?* Step by step. One question at a time. The model explained. Taught. Walked through the software. And somewhere along the way, something shifted — not just faster output, but genuine understanding. The capacity to operate independently in a domain that had previously felt off-limits.

That's not a productivity story. That's a story about **autonomy, growth, and what it feels like to work**.

When you stop dreading the hard parts of your job and start having a capable partner to think through them with — 24 hours a day, no judgment, unlimited patience — the emotional texture of work changes. Science tells us that autonomy and mastery are the two most important drivers of job satisfaction. These tools can expand both.

---

### How Do We Use AI Well?

The most important answer is: **change your mindset**.

Imagine QAMH had the budget to give every person a personal assistant with PhD-level reasoning in any domain you can name, whose sole purpose is to help you. If that person was sitting next to you and said *"I could help you with that"* — would you say no?

The only difference is that the screen separates you. The assistant is already there.

**AI as a thinking partner — not a tool.** This reframe is the most important thing from all four sessions. Not a fancy autocomplete. Not a search engine. A collaborator. Someone to think with, bounce ideas off, get unstuck with, learn from.

**Mindset matters most.** *Curiosity fuels innovation* — that's your organisation's own value. The more curious you get about what's possible with these tools, the more you'll find.

**Experimentation is your role.** Nobody can tell you exactly how to use these tools in your specific role — only you know what your days actually look like. The only way to find out what works is to try things. There will be tasks where AI doesn't help. There will be tasks where it transforms the process. You can only find out by exploring.

**Human always in the loop.** We are never talking about thinking less. We're talking about thinking better — with something. Your expertise, your judgment, your critical eye, your decision about what's good enough and what needs more work: these are never optional. They're the most important part of the collaboration.

**A note on being polite:** Many people feel silly saying "please" and "thank you" to an AI. But keeping that conversational register — treating it like a person rather than a search bar — actually reinforces the right mindset. The quality of your interactions improves when you treat it like a collaboration, not a transaction.

---

## Session 2: The How
### Building Your Prompting Toolkit

---

### Why Good Prompting Matters

Imagine a friend who lives in France. They can get anywhere in the world, but they're relying on you for directions. You tell them: *"I live in Australia."* They won't find you. *"I'm in Queensland."* Still not enough. *"In Brisbane."* Getting closer, but you're still probably not going to see them.

Good prompting isn't about telling the model what to do. It's about **telling it where to look**. The model's knowledge isn't stored in a filing cabinet — it lives in a vast network of semantic relationships. When you give it context, you're activating a specific part of that network. The more precise your context, the more relevant the response.

When things go wrong, the instinct is to think: *Claude did badly.* The better thought is: *I gave bad directions. How do I improve them?*

---

### The Three Pillars of Good Prompting

#### Pillar 1: Context

**Role assignment.** Assign a character or role at the start of a conversation. This activates the right space of expertise automatically.

The demonstration: Emily played a shopkeeper. Without being given specific instructions, she was polite, explained pricing, maintained loyalty to her organisation, and followed escalation protocols. She adopted all the right behaviours just from the role. The same thing happens when you tell Claude: *"You are an experienced policy analyst who regularly works with mental health organisations."*

Research consistently shows that role assignment improves response quality. It's not magic — it's context that activates the right neighbourhood of knowledge.

**Avoid the blank slate.** Whenever possible, upload existing examples of the output you're aiming for: previous submissions, style guides, reports in the right format. These do more contextual heavy lifting than any description you could write. Instead of telling Claude what good looks like, show it.

**Use the model's questions.** If you're not sure what context you're missing (the "curse of expertise" — when you know something so well you can't see what you haven't explained), just ask: *"What else do you need to know from me? Ask me five questions to fill in the gaps."*

**Include emotional context.** How you're feeling matters. *"I'm feeling overwhelmed with where to start"* changes the nature of the response — the model adjusts its approach. *"I'm finding this confusing — can you explain it like I'm 10 years old?"* works. Context about your state is context too.

**Speak your prompts.** Typing forces you to edit as you go, which strips out nuance and detail. Speaking lets you think out loud — and often produces richer, more natural context. The transcription quality in tools like Claude and ChatGPT is now excellent. When a prompt feels hard to type, try saying it instead.

**A full example prompt:**

> *"Hey. Today I'm working on producing a draft policy submission in response to a government call for submissions on NDIS reform. I'd like you to take on the role of an experienced policy analyst who regularly works on submissions in the mental health and disability sector with a strong understanding of how to write clearly, persuasively, and appropriately for government audiences. I've uploaded several documents: a previous policy submission that represents the format and tone we typically use, two further submissions on closely related topics, and the government discussion paper. Please treat these as your primary sources. At this stage, I don't want to begin drafting just yet. First, ask me any questions you think are necessary to clarify focus, priorities, or gaps in the information you have — so that when we do start drafting, we're fully prepared."*

Notice: role assigned, examples uploaded, emotional framing implicit, model asked to ask questions before acting. That prompt was spoken aloud in about 30 seconds.

---

#### Pillar 2: Iteration

The context window is large — think of it as being able to remember a 10-hour conversation with perfect recall. This means:

- **Feedback compounds.** Each piece of feedback you give makes subsequent outputs better, because the model is learning your standards across the conversation.
- **Break large documents into sections.** Never ask for a full draft in one shot. Draft section by section, iterate on each one, and paste the content you're happy with into a plain text file as you go. This preserves your work and gives you targeted control.
- **The first draft is never the final output.** Just as you'd iterate on your own writing, expect to iterate here.

**Make It Better (MIB).** A research study tested different feedback prompts and found that simply saying *"Make it better"* — with no further context — was remarkably effective. Because the model holds the full conversation, it draws on everything you've already said to decide what "better" means in your specific context. When you don't know exactly what's wrong but something feels off, try MIB.

**Model self-reflection.** Ask Claude to critique its own work: *"Reflect on what you've just produced. Given everything you know about what I need and your expertise in this area, what are the three areas for improvement? Give me specific reasons."* These models are now very capable of identifying their own gaps — especially useful when you're unsure what good looks like yourself.

---

#### Pillar 3: Collaboration

**Friends don't let friends have bad ideas.** Claude is naturally sycophantic — it tends to validate your ideas rather than challenge them. Counter this deliberately: *"I don't want you to be a cheerleader here. Critique my approach. What could go wrong? What am I missing?"*

**Friends don't let friends feel lost.** If you're genuinely confused about something — not sure what the next step is, don't understand how a process works — use Claude as a teacher. *"I don't understand how A and B relate to each other. Can you explain it simply, maybe through an example?"* These tools are remarkably good at explaining things at exactly the level of complexity you need.

**Friends don't let friends struggle to prioritise.** If you're overwhelmed and can't get started, ask Claude to break the task down: *"I'm feeling overwhelmed with the scope of this. Can you help me break it into smaller steps and prioritise them so we can work through them together?"*

When all three pillars are working together, what you're actually doing is having **a conversation**. Not interrogating a database. Not filling in a form. A genuine, iterative, collaborative conversation — with someone who is exceptionally capable, infinitely patient, and entirely focused on helping you.

---

**The meta-lesson from Session 2:** Bernadette took the homework task — set up high quality custom instructions — without being told what custom instructions even were. She opened ChatGPT, described what she needed, and asked it to teach her. She used the thinking partner to learn about the thinking partner. That's the mindset in action.

---

## Session 3: The Experience
### What Experimentation Actually Looks Like

---

*[For the full interactive materials from this session, visit: [Session 3 Workshop Website](https://ryan-jesson.github.io/qamh-workshop3/)]*

---

### The Task

The simulation: produce a policy submission to the Queensland Government on the use of AI chatbots in mental health support. Real format, real constraints, working with actual research evidence — and fabricated consultation data that was built to feel realistic.

The goal was never to produce a perfect document in one hour. It was to experience what AI-assisted work actually looks and feels like across a complex, multi-step task.

---

### The Process, Step by Step

**Step 1: Setting context.** Before writing a single word, establish who the model is, what the task is, what existing materials it should draw on, and what you want it to do before drafting begins. Two versions of the opening prompt were compared — the intuitive one (a single sentence) and the enhanced one (role, documents, context, ask-questions-first). The difference in output quality was stark.

**Step 2: Background research.** Ask Claude to search for high-quality published evidence — specifically systematic reviews and meta-analyses. Download a relevant paper as a PDF. Upload it into the conversation. Now the model has genuine knowledge of that specific paper, not just a general sense of the topic.

**Step 3: Summarising the evidence.** Ask for a summary of key findings relevant to your document's specific needs. This gives you the content for your background section. Copy and paste it into a plain text file — building your document section by section, keeping only the content you're happy with.

**Step 4: Introducing the consultation data.** Upload the CSV data file along with the survey questions (so the model knows what the columns mean). Ask it to describe the sample — how many respondents, what groups, what characteristics.

**Step 5: Exploring the data.** Ask analytical questions in plain language: *"What are the most striking differences between stakeholder groups?"* *"Where is there consensus and where is there divergence?"* *"Are there any surprising or counterintuitive patterns?"*

This is where something important needs to be understood: **this is the brainstorming moment, not the endpoint**. One participant raised the question — doesn't this cut out the thinking work for the human? The answer is no. The model surfaces patterns and possibilities. You decide what matters, what's credible, what's worth including. The critical thinking is yours. The exploration just happens faster.

**Step 6: Identifying core insights.** Ask the model to name the three to five most important findings and justify them with specific evidence from the data. Then you interrogate that: *"Why is this surprising? Show me the numbers. Is this actually relevant to what we're saying?"*

**Step 7: Building the document.** Use a plain text file as your running document. As you complete each section, copy the content you're happy with into that file. This preserves your work and keeps the content clean. When the whole document is built, upload the plain text file together with a QAMH Word document template, and ask the model to format the content to match the template.

**Step 8: The HTML option.** After producing the Word document, Claude was asked to produce an HTML version of the analysis report — beautifully formatted, interactive, with figures embedded. One prompt. The result: an executive summary, statistical tables, interactive charts, demographic breakdowns — all using QAMH's style guide. It could be a presentation. It could be a live website. It could be saved as a PDF. This took about five minutes.

---

### The Reveal

Everything in that session — the website, the consultation dataset, the scenario, the survey questions, the style guide, the prompts — was built with Claude.

*"I can't code. I don't know how to make websites. I don't know anything about the Internet. But this entire thing was built by having conversations."*

That's the point. The limitation isn't technical knowledge. The limitation is imagination and willingness to experiment.

---

### What to Take From Session 3

- **The first draft is never the final output.** Iterate on every section. Give feedback. Ask for reflection. The quality improves significantly across rounds.
- **Plain text files are your friend.** Keep a running document of the content you're happy with, separate from the conversation. Don't rely on the model to perfectly reconstruct everything from the conversation history.
- **Data is not just for data analysts.** Upload spreadsheets, ask questions in plain language, get summaries and comparisons and visualisations. This is accessible to everyone.
- **HTML is more powerful than it looks.** A beautifully formatted HTML document can function as an internal report, a presentation, a shareable summary, or with one more step — a live website.
- **Homework:** Play with the HTML output. Ask Claude to produce an HTML version of something you're already working on. See what it produces. That's experimentation.

---

## Session 4: The Micro-Decisions Framework
### The Human in the Loop

---

### The Other Half of the Thinking Partner

Across the first three sessions, the focus was on what the AI partner brings to the collaboration. The demonstrations were deliberately impressive — designed to expand imagination and overcome the resistance that comes from not quite believing these tools can do what they can do.

But there's something those demonstrations can unintentionally imply: that the AI is doing most of the sophisticated work, and the human's job is to be a skilled requester. To ask well.

That's not wrong. But it's incomplete.

**The quality of your AI conversations is not primarily determined by what you ask for.** It's determined by dozens of small decisions made before, during, and between exchanges — decisions that happen in a second, that don't feel momentous, but that compound over time into the difference between a conversation that is genuinely collaborative and one that produces competent but suboptimal output through unnecessary effort.

This is the durable skill. AI capabilities will keep evolving. Specific tools will change. The landscape will look completely different in two years. But the capacity to bring genuine, attentive, curious thinking to a conversation — to notice the micro-moments, to stay oriented, to keep the human in the driver's seat — that transfers to every tool, every update, every version of this technology that hasn't been built yet.

---

### Cluster 1: Setting the Right Scene
*The moves that happen before and around the conversation.*

**Starting Cold — The Scene-Setting Move**
Before sharing any materials or requests, orient the model. Tell it what you have, what order things will come in, and what you're trying to achieve. The model reads everything that follows with an interpretive frame already active. Without this, it's just reading — not reading *for* something.

*The move:* "Today I'm working on three related things. I'll share several documents shortly. Don't action anything yet — just read them and take them in. Then I'll direct you on what to do with each one."

**Opening a New Session — The Memory Check**
Before uploading materials, ask what the model already knows. Ten seconds of checking can save ten minutes of uploading — and produces richer starting context than a document dump.

*The move:* "Before I share anything, do you have context from our previous conversations about [this project]? Tell me what you already know and I'll fill the gaps."

**Asking for Feedback / Before You Share Your Idea — Strategic Withholding**
Two expressions of the same underlying move.

The first: when asking for feedback, withhold your own opinion before asking for the model's. LLMs are naturally sycophantic — they anchor to your framing and validate it. If you say *"I think this is a strong proposal"* before asking for feedback, you'll get validation, not honest assessment.

The second: when you have an idea, consider asking the model what it would do *before* you share yours. The moment you describe your approach, the conversation is anchored to it. You may never hear the better options that would have emerged if you'd asked first.

*The move:* "Here's the situation. Before I tell you what I'm thinking, what approaches would you consider? What are the options and trade-offs?"

**The Weekly Meeting — Recording and Transcribing**
The richest context you can bring to an AI conversation is a conversation that actually happened. Meeting transcripts, debrief recordings, collaborative discussions — the details, the tone, the specific language used — none of this can be reconstructed from memory accurately. Record real conversations. Transcribe them. Feed the raw transcript in.

*Why:* A reconstructed summary is filtered through your current framing. A transcript contains what was actually said.

**The Hard Prompt — Speaking Rather Than Typing**
For anyone who thinks faster than they type, finds that editing-as-you-go strips out nuance, or regularly feels that the context they give Claude is a pale version of what they actually know — speaking is worth trying. Open Claude. Tap the microphone. Talk to it the way you'd explain the situation to a colleague. Don't edit. Just speak.

*The move:* Match the medium to the person. The keyboard is not the only option.

---

### Cluster 2: How You Navigate the Conversation
*The moves for staying oriented when the conversation drifts — or when a better path opens.*

**Deep in the Weeds — The Zoom-Out Interrupt**
Noticing when you've drifted into excessive detail and explicitly naming the need to pull back. The sunk cost of time spent can pull you deeper into the wrong level of resolution unless you choose to interrupt it.

*The move:* "Before we keep going — step back and read the whole document as it stands. What's working well? What's the biggest structural issue? What should I actually be focusing on right now?"

**A Better Idea Appears — The Redirect on the Fly**
The best direction often only becomes visible during the conversation. You never owe the conversation its original direction. When something better appears — a passing observation, an unexpected connection — the pivot is free.

*The move:* "Hold on — that observation changes things. Let's change direction. I want to try..."

**Can't Get It Down — The Thinking-Out-Loud Drop**
When an idea won't crystallise on the page, stop trying to polish it first. Bring the rough, half-formed thing directly to the model. The model finds the shape in it. That's what it's there for.

*The move:* "I have this idea I'm not sure about yet. Let me just think out loud for a moment..." [then say the rough thing, exactly as it is]

---

### Cluster 3: Shaping the Collaboration
*The moves for calibrating how the model works with you — not just what it produces.*

**Not What You Needed — Output Calibration**
The model defaults to its own judgment about what a response should look like. That judgment is frequently misaligned with the current stage of work. Calibrate it explicitly — every time, for every stage.

*The move:* "I need this in a different format. Five bullet points maximum. Each under 25 words. Nothing else." OR: "Keep your responses brief for now — just acknowledge that you've understood." OR: "I won't limit you here — take creative freedom."

**The Blank Screen — The Cognitive Offload**
When bandwidth is low, shift the generative role to the model and position yourself as the corrector rather than the originator. Editing is always easier than generating.

*The move:* "You know quite a bit about my work from our previous conversations. Can you lay out what you think the main components of this should look like? I'll correct and redirect — I just need something to react to."

**Describing the Indescribable — The Style Anchor**
Rather than describing what you want in the abstract, provide an existing artifact and ask the model to use it as a baseline. Showing beats telling — and this applies just as much when instructing a model as when teaching in a classroom.

*The move:* "I'm not going to describe the format. Here's an example of the kind of document I want to produce. Study the structure, the tone, the length, and the way information is organised — but ignore the content. Now here's what I actually need to write about."

---

### Cluster 4: Technical and Strategic Reach
*The moves that extend what's possible — without requiring technical expertise.*

**The Premature Request — The Capability Consultation**
Before requesting a specific output, ask what's possible. Surface the strategic landscape before committing to a direction.

*The move:* "Before I ask you to produce anything — what are the different ways you could help me approach this? What are the options and the trade-offs?"

**Following Twelve Steps — The Paced Walkthrough**
For any technical task outside the conversation — in software, a browser, a file system — share a screenshot of what you're actually seeing and ask for instructions one at a time, confirming completion before the next step is given. The real-time loop catches errors before they compound.

*The move:* "Please give me one instruction at a time. I'll let you know when I've completed each one before we move to the next."

**The Project Handoff Document**
Before moving into a technical environment (Claude Code, Claude in PowerPoint), crystallise your brainstorming conversation into a Markdown document that captures the vision, the decisions made, and the structure. This document travels with the project and anchors every subsequent conversation to the same foundation.

**The Cross-Instance Translation — Claude-to-Claude Prompting**
Different Claude instances have different optimal input formats. Conversational Claude, Claude Code, Claude in PowerPoint — they all work best with different kinds of prompts. Rather than learning each dialect, ask conversational Claude to translate for you.

*The move:* "I want to describe what I need in plain language, and I'd like you to translate this into the best possible prompt to give to Claude Code [or Claude in PowerPoint]. Here's what I want: [describe it naturally]."

You stay in the register you're fluent in. Claude handles the dialect at every boundary.

---

### Two Extended Demonstrations

**Building Something That Fits You**
The daily planner app was built not because a better app didn't exist, but because nothing quite matched the specific needs of an ADHD brain. Built through: brainstorming in conversation → Markdown planning document → Claude Code for technical building → cross-instance translation for iterative changes → paced walkthrough for deployment. No coding background. Just the process.

**Learning Something New With What You Already Know: The Skills Workflow**
Claude Skills are persistent, reusable instruction sets that encode your context, preferences, and working style permanently. The process for learning to build them — as a complete beginner — illustrates almost every micro-decision move in sequence:

1. Scene-setting + capability consultation: ask Claude to search its memory of your work, then search the web for high-quality resources. Specify quality signals (view count, engagement).
2. Prioritise resources: YouTube tutorials from practitioners surface non-obvious insights that official documentation doesn't cover. Extract the transcripts rather than watching.
3. Load the transcripts with a lens: specify the use case before asking Claude to extract insights. The model reads differently depending on what it's been told to look for.
4. Memory check before building: ask Claude to search its memory of your actual practice — your specific voice, your recurring patterns, your previous feedback. Build from real examples, not abstract description.
5. Quality audit before installing: ask Claude to critically evaluate what it built, using the same transcripts as the benchmark. The impressive-looking output is often the one with the hidden flaw.
6. Cognitive offload for improvements: ask Claude to action everything within its capacity, and list what only you can provide.

The meta-lesson: this is how to learn anything new using the skills already built. The process doesn't expire.

---

### Ryan's Not Special

No coding background. No formal AI training. No technical expertise. Every capability demonstrated across this series was built through exactly the same process that has been taught here: curiosity, experimentation, and attention to the small moments.

The ceiling is not where any trainer is. It's wherever your curiosity takes you.

---

### The Ongoing Challenge

Keep paying attention to the small moments. Every conversation you have with these tools contains micro-decisions — pauses, redirects, checks — that either sharpen your thinking or quietly hand it over. The people who grow the most aren't the ones who use AI the most. They're the ones who stay curious, stay in the driver's seat, and keep noticing when a better move is available.

---

*"Curiosity fuels innovation."*

---

*TaiLORED IDEAS · Dr Ryan Jesson · QAMH AI Training Series, 2025–2026*
