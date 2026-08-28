# Portfolio Case Studies

## Voice Card
**Direct, warm, plain-spoken, not stiff.**
*(Standing instruction — check every line against this before it goes live.)*

---

## Case Study: Hands-Free Repair Logging Agent

**The Problem**

Electronics repair techs work with their hands full — mid-repair, they'll spot something that needs replacing or recording, but stopping to type it out breaks their flow. Worse, by the time they're done fixing the device, they've often forgotten the exact detail: which capacitor, what the symptom was, what they decided to do about it. I wanted to build something that lets them capture that information the moment they notice it, without putting down the tool in their hand.

**What I Did**

I'm building an AI agent that connects to a database with full create, read, update, and delete permissions — controlled, not automatic. Right now it's a working proof of concept, not the full system: I click a microphone button, say what I'm seeing (like a replaced part or a symptom), and the system transcribes it, stores it in a structured table, and can recall and make inferences from what's been logged.

A few decisions I made on purpose:
- **Local database (DBeaver), not cloud.** This is a single-user tool for one repair tech, not a large-scale system — so I kept the infrastructure as simple as the problem actually needed.
- **Confirm-before-execute.** The agent logs the command first and only creates, updates, or deletes a row once the user approves it. I didn't want an AI agent making irreversible changes to someone's data without a human in the loop.
- **Scoped down on purpose.** I built the proof of concept as a chatbot with memory first, before attempting the full hands-free agent. It's not fully voice-activated yet — I still click a button to record instead of a wake word — and I'd rather be honest about that than oversell it.

**What Came Of It**

The system works end to end: it captures spoken input, stores it as structured data, and can recall and reason over past entries. It's not fully hands-free yet — that's the clear next step. The biggest thing I learned building this so far is how much of the work is invisible: the research and planning took roughly three times longer than the actual building. Scoping a system down to something achievable turned out to be a bigger skill than writing the code itself.

---

## Bio

I'm an Information Systems student building practical tools at the intersection of AI, databases, and real-world workflows. Alongside my coursework, I'm active in university career services and social media, and I'm currently learning C++, Kali Linux, and core computer science fundamentals. I like projects that solve a specific, unglamorous problem for a specific person — like giving a repair tech their hands back.

## Contact / CTA

Want to see how this agent evolves, or talk through a project? Reach out — amukelani.mabunda16@gmail.com ·(https://github.com/amuk86)

---

## Before / After: Catching the "AI Voice"

**Generic AI line (what a model would default to):**
> "This innovative AI-powered solution leverages cutting-edge natural language processing to seamlessly streamline the repair documentation workflow, empowering technicians to focus on what matters most."

**Your edited version:**
> "Repair techs shouldn't have to stop mid-fix to write things down. This agent lets them just say what they're seeing, and it gets logged — so nothing gets forgotten and nothing gets in the way."

*What changed: cut "innovative," "cutting-edge," "leverages," "seamlessly," "empowering" — all filler that could describe any product. Replaced it with the actual person (a tech, mid-fix) and the actual outcome (nothing forgotten, nothing in the way).*
