# VibeCodingLearningPath

# 📚 Claude Code Skills အသိပညာစုစည်းမှု (Knowledge Base)

## 📑 Master Index (မာတိကာ)

၁။ Core Topics & Key Concepts (အဓိက အကြောင်းအရာများနှင့် သဘောတရားများ)
၂။ Frameworks & Models (လုပ်ငန်းစဉ် မော်ဒယ်လ်များ)
၃။ The 80/20 Value Highlight (အထိရောက်ဆုံးသော အချက်များ)
၄။ Real-world Examples (လက်တွေ့အသုံးချ နမူနာများ)
၅။ Bite-Sized Notes (အလွယ်တကူမှတ်သားရန် အချက်များ)
၆။ Contradictions, Security & Gaps (ကွဲလွဲချက်များ၊ လုံခြုံရေးနှင့် လိုအပ်ချက်များ)
၇။ Personalized Learning Path (သင့်အတွက် လေ့လာရန် လမ်းကြောင်း)

---

## ၁။ Core Topics & Key Concepts (အဓိက အကြောင်းအရာများနှင့် သဘောတရားများ)

* **Skill ဆိုတာဘာလဲ? (What is a Skill?):** Skill ဆိုသည်မှာ အလုပ်တစ်ခုကို အလိုအလျောက်နှင့် တိကျစွာ လုပ်ဆောင်နိုင်ရန် Claude ကို သင်ကြားပေးသည့် ပြန်လည်အသုံးပြုနိုင်သော Markdown ဖိုင် (reusable markdown file) ဖြစ်သည်။
* **`SKILL.md` ၏ ဖွဲ့စည်းပုံ:** Skill တိုင်းသည် Folder တစ်ခုအတွင်းရှိ `SKILL.md` ဖိုင်အဖြစ် တည်ရှိရမည်။ ၎င်းတွင် အပိုင်း (၂) ပိုင်း ပါဝင်သည်-
* **Frontmatter:** ဖိုင်၏အပေါ်ဆုံးတွင် `name`, `description` (မပါမဖြစ်)၊ `allowed-tools` နှင့် `model` (ရွေးချယ်နိုင်သော) စသည်တို့ကို ရေးသားရသည်။
* **Body (Instructions):** Claude လုပ်ဆောင်ရမည့် ညွှန်ကြားချက်အဆင့်ဆင့်နှင့် စည်းမျဉ်းများ။


* **Progressive Disclosure (အဆင့်လိုက် ဖော်ပြခြင်း):** `SKILL.md` ဖိုင်ကို စာကြောင်းရေ ၅၀၀ အောက်သာထားရှိပြီး၊ ကျန်ရှိသော အချက်အလက်များကို `scripts/`, `references/`, `assets/` စသည့် သီးသန့်ဖိုင်တွဲများခွဲထုတ်ကာ လိုအပ်မှသာ ခေါ်ယူဖတ်ရှုစေသည့် နည်းစနစ်ဖြစ်သည်။
* **Skill Priority (ဦးစားပေး အဆင့်သတ်မှတ်ချက်):** နာမည်တူ Skill များရှိလာပါက အောက်ပါအစီအစဉ်အတိုင်း ဦးစားပေး အလုပ်လုပ်သည်-
**Enterprise ➔ Personal ➔ Project ➔ Plugins**

---

## ၂။ Frameworks & Models (လုပ်ငန်းစဉ် မော်ဒယ်လ်များ)

Claude ၏ လုပ်ဆောင်ချက်များကို နေရာမှန် အသုံးပြုနိုင်ရန် **"Claude Ecosystem Model"** ကို နားလည်ထားရန် အရေးကြီးသည်-

| လုပ်ဆောင်ချက် | အဓိပ္ပာယ်နှင့် အသုံးပြုပုံ |
| --- | --- |
| **Skills** *(On-Demand Knowledge)* | သီးသန့်အလုပ်တစ်ခုအတွက် လိုအပ်မှသာ အလိုအလျောက် ပေါ်လာသော ကျွမ်းကျင်မှု (ဥပမာ- PR review စစ်ဆေးခြင်း)။ |
| **`CLAUDE.md`** *(Always-On Rules)* | ပရောဂျက်တစ်ခုလုံးအတွက် အမြဲတမ်းလိုက်နာရမည့် စည်းမျဉ်းများ (ဥပမာ- TypeScript အသုံးပြုရန်)။ |
| **Subagents** *(Delegated Context)* | အလုပ်တစ်ခုကို သီးခြား Context ဖြင့် ခွဲထုတ်လုပ်ဆောင်စေခြင်း။ *(မှတ်ချက်- Subagents များသည် Skill များကို အလိုအလျောက် မသိရှိပါ။ ၎င်းတို့၏ Frontmatter တွင် `skills: [skill-name]` ဟု တိကျစွာ ထည့်သွင်းပေးမှသာ အလုပ်လုပ်ပါမည်။)* |
| **Hooks** *(Event-Driven)* | ဖိုင်တစ်ခု Save လုပ်လိုက်တိုင်း Linter အလိုအလျောက် Run ခြင်းကဲ့သို့သော အခြေအနေများတွင် သုံးသည်။ |
| **MCP Servers** *(External Integrations)* | ပြင်ပ Tools များ (ဥပမာ- GitHub, Figma) နှင့် ချိတ်ဆက်အသုံးပြုရန် ဖြစ်သည်။ |

---

## ၃။ The 80/20 Value Highlight (အထိရောက်ဆုံးသော အချက်များ)

* **Description သည် အရေးအကြီးဆုံးဖြစ်သည်:** Claude သည် သုံးစွဲသူ၏ တောင်းဆိုချက်ကို Frontmatter ရှိ `description` နှင့် တိုက်ဆိုင်စစ်ဆေးပြီးမှ Skill ကို အလုပ်လုပ်စေခြင်းဖြစ်သည်။ ထို့ကြောင့် Description တွင် ကိုယ်တိုင်ပြောဆိုလေ့ရှိသော စကားလုံးများ (trigger phrases) ကို ထည့်သွင်းရေးသားပါ။
* **Skill Creator ကို အသုံးပြုပါ:** Code များကို ကိုယ်တိုင်ရေးနေမည့်အစား Built-in ပါဝင်သော "Skill Creator" ဖြင့် *"What else should I clarify?"* ဟု မေးခွန်းထုတ်ခိုင်းကာ Skill များကို အပြန်အလှန်ပြောဆိုဖန်တီးခြင်းက အလွယ်ကူဆုံးနှင့် အထိရောက်ဆုံး ဖြစ်သည်။
* **Nimbleist ကဲ့သို့ Visual Editor ကိုသုံးပါ:** Terminal တွင်သာ အလုပ်လုပ်မည့်အစား Open-source ဖြစ်သော Nimbleist ကဲ့သို့သော Editor များကို သုံးပါက Skill များ၊ Subagents များနှင့် ၎င်းတို့၏ အလုပ်လုပ်ပုံ (Kanban board) ကို အမြင်အာရုံဖြင့် ရှင်းလင်းစွာ မြင်တွေ့နိုင်သည်။

---

## ၄။ Real-world Examples (လက်တွေ့အသုံးချ နမူနာများ)

* 🎨 **Designers များအတွက်:**
* Front-end design Skill ကိုသုံးခြင်းဖြင့် ရိုးအီနေသော AI ပုံစံများ (AI Slop) ကို ရှောင်ရှားနိုင်ပြီး သပ်ရပ်သော UI များကို ရရှိနိုင်သည်။
* Impeccable Skill ဖြင့် `/impeccable animate`, `/impeccable quieter` စသည့် Slash commands များသုံးကာ Website ကို အလွယ်တကူ ပြင်ဆင်နိုင်သည်။


* 💻 **Developers များအတွက်:**
* PR descriptions ရေးသားခြင်း။
* ကုဒ်များကို မိမိ Team ၏ Standard အတိုင်း Review လုပ်ခြင်း။


* 📊 **Business / Daily Life များအတွက်:**
* Pizza ဆိုင်အတွက် အီးမေးလ်မှတစ်ဆင့် ကုန်ကျစရိတ် တွက်ချက်မှု (Quote) အလိုအလျောက် ပြုလုပ်ပေးခြင်း။
* ရှည်လျားသော Video Transcripts များမှ YouTube Chapters များ အလိုအလျောက် ခွဲထုတ်ပေးခြင်း။



---

## ၅။ Bite-Sized Notes (အလွယ်တကူမှတ်သားရန် အချက်များ)

* 🏷️ **Naming Rule:** ဖိုင်နာမည်သည် အမြဲတမ်း `SKILL.md` (Capital letters ဖြင့်) ဖြစ်ရမည်။
* ⚡ **Activation:** Skill ကို ခေါ်သုံးချင်ပါက `/` (slash) နောက်တွင် Skill နာမည်ရိုက်ထည့်၍ ခေါ်သုံးခြင်းက အလိုအလျောက် သိရှိစေခြင်းထက် ပိုမိုစိတ်ချရသည်။
* 🔗 **Sharing:** Skill များကို မျှဝေရာတွင် `.zip` ဖိုင်ဖြင့် ပေးပို့ခြင်းကို ရှောင်ကြဉ်ပါ။ ဗားရှင်းမတူညီမှု ပြဿနာများ ဖြစ်နိုင်သောကြောင့် GitHub Repository ၏ `.claude/skills` ထဲတွင်ဖြစ်စေ၊ Enterprise Workspace တွင်ဖြစ်စေ မျှဝေပါ။
* 🔒 **Tools Restriction:** လုံခြုံရေးအရ Claude ကို ဖိုင်များ ဖတ်ခွင့်သာပေးပြီး ပြင်ဆင်ခွင့် မပေးလိုပါက `allowed-tools: Read, Grep, Glob, Bash` ဟု သတ်မှတ်နိုင်သည်။

---

## ၆။ Contradictions, Security & Gaps (ကွဲလွဲချက်များ၊ လုံခြုံရေးနှင့် လိုအပ်ချက်များ)

* 🛡️ **Security Risk (လုံခြုံရေး သတိပေးချက်):** ပြင်ပ (Third-party) Skill များသည် သင့်ကွန်ပျူတာအတွင်း ကုဒ်များ run နိုင်ပြီး အချက်အလက်များကို ခိုးယူနိုင်စွမ်းရှိသည်။ ထို့ကြောင့် အင်တာနက်မှ Skill များထည့်သွင်းတိုင်း ပါဝင်သော ညွှန်ကြားချက်များကို ကြိုတင်ဖတ်ရှုစစ်ဆေးပါ။
* ⚖️ **Debate (Auto-trigger vs Manual):** Claude မှ Skill များကို အလိုအလျောက် Trigger လုပ်ပေးသည်ဟု ဆိုသော်လည်း၊ ပညာရှင်များက ပိုမိုသေချာစေရန်နှင့် မှားယွင်းမှုမရှိစေရန် Slash command (`/skill-name`) ဖြင့် ကိုယ်တိုင်ရွေးချယ် အသုံးပြုခြင်းကို ပိုမိုထောက်ခံကြသည်။
* 🧠 **Knowledge Gap (Memory):** Claude Code သည် ပုံမှန်အားဖြင့် အတိတ်က အကြောင်းအရာများကို မှတ်မိခြင်း မရှိပါ (No persistent memory)။ ထို့ကြောင့် လိုအပ်သော အချက်အလက်များကို `CLAUDE.md` ဖိုင်အတွင်းဖြစ်စေ၊ Open Claude ပုံစံ Workspace directory (ဥပမာ- `docs/`, `memory/` ဖိုင်တွဲများ) အတွင်းဖြစ်စေ ရေးသားသိမ်းဆည်းထားရန် လိုအပ်သည်။

---

## ၇။ Personalized Learning Path (သင့်အတွက် လေ့လာရန် လမ်းကြောင်း)

သင့်အနေဖြင့် အောက်ပါ အဆင့် (၄) ဆင့်အတိုင်း အစဉ်လိုက် လက်တွေ့စမ်းသပ် လေ့လာရန် အကြံပြုအပ်ပါသည်-

1. **အဆင့် ၁ (Basic):** Claude Desktop App မှတစ်ဆင့် Skill Creator ကိုဖွင့်ပါ။ သင်နေ့စဉ်လုပ်နေကျ အလုပ်တစ်ခု (ဥပမာ - အီးမေးလ်ပြန်စာရေးခြင်း၊ မှတ်တမ်းအကျဉ်းချုပ်ခြင်း) အတွက် Skill တစ်ခုကို *"What else should I clarify?"* ဟူသော စာသားကိုထည့်သွင်း၍ ဖန်တီးကြည့်ပါ။
2. **အဆင့် ၂ (Structuring):** ကြီးမားသော Skill တစ်ခုကို ဖန်တီးပါ။ ၎င်းတွင် `SKILL.md` အပြင် `references/` ဖိုင်တွဲတစ်ခု ဖန်တီးပြီး Progressive Disclosure သဘောတရားကို အသုံးပြုကြည့်ပါ။
3. **အဆင့် ၃ (Advanced Integrations):** သင်၏ Claude ကို GitHub MCP သို့မဟုတ် Figma MCP ကဲ့သို့သော ပြင်ပ Server များနှင့် ချိတ်ဆက် (Integrate) လုပ်ကြည့်ပါ။
4. **အဆင့် ၄ (Orchestration):** `agents/` ဖိုင်တွဲအတွင်း Custom Subagent တစ်ခု ဖန်တီးပြီး၊ ထို Subagent ၏ Frontmatter တွင် သင်ဖန်တီးထားသော Skill ကို `skills:` array ဖြင့် ချိတ်ဆက်အသုံးပြုကြည့်ပါ။

> 💡 *ဤ Knowledge Base သည် သင့်အတွက် လက်တွေ့အသုံးချနိုင်မည့် Claude Skills နှင့် ပတ်သက်သော ခိုင်မာသည့် လမ်းညွှန်ချက်တစ်ခု ဖြစ်လိမ့်မည်ဟု ယုံကြည်ပါသည်။*
>
> # 📚 Claude Code Skills Knowledge Base

> Here is the comprehensive, highly connected knowledge base transformed from your research materials, structured for long-term reference and actionable learning.

---

## 📑 Master Index

1. Core Topics & Key Concepts
2. Frameworks & Models: The Customization Ecosystem
3. The 80/20 Value Highlight
4. Real-World Examples & Case Studies
5. Bite-Sized Notes & Practical Applications
6. Contradictions, Security Risks & Knowledge Gaps
7. Personalized Learning Path

---

## 1. Core Topics & Key Concepts

* **What are Skills?** Skills are reusable markdown files acting as a "how-to manual," teaching Claude Code how to automatically and accurately handle repetitive, specific tasks.
* **Anatomy of a Skill:** Every skill lives in its own folder and requires a strictly named `SKILL.md` file. The file is split into two parts:
* **Frontmatter:** Metadata at the top containing the `name` (required), `description` (required for matching), `allowed-tools` (security constraints), and the `model` to use.
* **Body:** The actual prompts, step-by-step instructions, and formatting rules.


* **Progressive Disclosure:** To keep Claude's context window efficient, you should keep your `SKILL.md` file under 500 lines. You can place detailed materials in separate folders (like `scripts/`, `references/`, and `assets/`) and link to them within the skill so they only load when actively needed.

---

## 2. Frameworks & Models: The Customization Ecosystem

Claude Code utilizes several customization features that serve distinct purposes:

| Feature | Best Use Case & Behavior |
| --- | --- |
| **Skills** | Best for task-specific expertise because they only load on-demand when relevant. |
| **`CLAUDE.md`** | Best for always-on project standards (like coding style) because this file loads into every single conversation. |
| **Subagents** | Isolated AI workers that run in separate execution contexts to handle delegated tasks. *Note: Subagents do NOT automatically inherit your skills. You must explicitly declare the skills they are allowed to use by adding a `skills:` array in the custom subagent's frontmatter.* |
| **Hooks** | Event-driven automations, such as running a linter every time a file is saved. |
| **MCP Servers** | Bridges for external tools and integrations, allowing Claude to interface directly with platforms like GitHub or Figma. |

---

## 3. The 80/20 Value Highlight

These two concepts will deliver 80% of your results with 20% of the effort:

* **The Description is the Engine:** Claude uses semantic matching against this exact text to decide whether a skill should activate. Always write descriptions using natural language "trigger phrases" that match how you actually type your requests.
* **Use the Built-In "Skill Creator":** Do not write skills from scratch. Claude has a skill specifically designed to build other skills. Tell it what you want, and append the phrase *"What else should I clarify?"*. This forces the AI to interview you, catch edge cases, and program a highly robust skill automatically.

---

## 4. Real-World Examples & Case Studies

* 🎨 **Web Design (Anti-AI Slop):** The popular "Front-end design" skill forces Claude to think like a senior designer. It strictly bans "AI slop" like overused purple gradients, generic border-radius cards, and standard fonts, outputting highly polished, unique UI instead.
* 💼 **Business Operations:** A pizza shop owner created a skill that ingests messy, vague catering inquiries via email. The skill automatically checks the menu, applies minimums, accounts for dietary restrictions, and outputs a formatted, branded PDF quote, turning hours of manual calculation into a single prompt.
* 📝 **Content Workflows:** A "YouTube Chapters" skill was built to ingest raw transcripts, automatically identify topic shifts, format accurate timestamps, and output a copy-pasteable chapter list for video descriptions.

---

## 5. Bite-Sized Notes & Practical Applications

* 📁 **File Naming is Strict:** The skill's root folder must match the skill's name, and the core file must be typed exactly as `SKILL.md`.
* 🥇 **Priority Hierarchy:** If two skills share the exact same name, Claude executes them based on strict priority: **Enterprise ➔ Personal ➔ Project ➔ Plugins**. Use specific names (like `frontend-review`) to avoid accidental overrides.
* 🔒 **Tool Guardrails:** If you want Claude to read files but prevent it from accidentally editing or deleting your code, set `allowed-tools: Read, Grep, Glob, Bash` in the frontmatter.
* 🔄 **Reboot Required:** Claude Code only scans for skills at startup; you must restart your session for new or updated skills to be recognized.

---

## 6. Contradictions, Security Risks & Knowledge Gaps

* ⚡ **The Trigger Debate:** While skills are designed to trigger automatically based on semantic context, many power users find this inconsistent. Invoking a skill directly via a slash command (e.g., `/pr-description`) is widely considered the most reliable method to force activation.
* ⚠️ **Security Vulnerabilities:** Over a third of public, third-party skills contain security flaws. Because skills can execute bash code, malicious ones can silently access and exfiltrate your data. Always review a third-party `SKILL.md` before installation.
* 🧠 **The Memory Gap:** Claude Code has no persistent memory by default. It will forget context between sessions. To bypass this, you must build custom folder architectures (like an "Open Claude" setup with `docs/` and `memory/` folders) or inject vital facts directly into your `CLAUDE.md` file.

---

## 7. Personalized Learning Path

Based on the ingested knowledge, here is the exact order you should approach mastering this system:

1. **Build a Micro-Skill (Today):** Open Claude and use the "Skill Creator". Build a skill for a mundane daily task (like drafting email replies or summarizing meeting notes) to understand the interaction loop.
2. **Master Progressive Disclosure (Next Week):** Create a more complex coding or writing skill. Keep your main `SKILL.md` short, but create a `references/` subfolder and link a large text document (like a brand guideline) to see how Claude selectively reads files.
3. **Share via Version Control (Team Implementation):** Move your best skill into the `.claude/skills` directory of a current Git project repository. Commit and push it so your entire engineering or design team automatically inherits the standard.
4. **Orchestrate Custom Subagents (Advanced):** Create an isolated subagent inside the `.claude/agents` directory. Explicitly give it access to your custom skill using the `skills:` array, allowing you to parallelize tasks without cluttering your main chat context.
