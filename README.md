# 🛡️ AI Penetration Testing | ML & LLM Security | Prompt Injection

Welcome to the **AI/ML/LLM Penetration Testing Toolkit** by [Mr-Infect](https://github.com/Mr-Infect) — the **#1 GitHub resource for AI security, red teaming, and adversarial ML techniques**. This repository is **dedicated to offensive and defensive security** for cutting-edge AI, Machine Learning (ML), and Large Language Models (LLMs) like ChatGPT, Claude, and LLaMA.

> ✅ Designed for **cybersecurity engineers, red teamers, AI/ML researchers, and ethical hackers**
> ✅ focused to : `AI Penetration Testing`, `Prompt Injection`, `LLM Security` , `Red Team AI`, `AI Ethical Hacking`

---

## 🌐 Why AI/LLM/ML Pentesting Matters in 2025

AI is now integrated across **finance**, **healthcare**, **legal**, **defense**, and **national infrastructure**. Penetration testing for AI systems is no longer optional — it is mission-critical.

### Common Threats:

* 🕵️ **Sensitive Data Leaks** – PII, trade secrets, source code
* 💀 **Prompt Injection Attacks** – Jailbreaking, sandbox escapes, plugin abuse
* 🧠 **Model Hallucination** – Offensive, misleading, or manipulated content
* 🐍 **Data/Model Poisoning** – Adversarial training manipulation
* 🔌 **LLM Plugin Abuse** – Uncontrolled API interactions
* 📦 **AI Supply Chain Attacks** – Dependency poisoning, model tampering

---

## 🚀 Get Started Fast

To use this repository effectively:

### Recommended Skill Set

* 🔬 Understanding of AI/ML lifecycle: `Data > Train > Deploy > Monitor`
* 🧠 Familiarity with LLMs (e.g. Transformer models, tokenization)
* 🧑‍💻 Core pentesting skills: XSS, SQLi, RCE, API abuse
* 🐍 Strong Python scripting (most tools and exploits rely on Python)

---

## 📚 Repository Structure 

### 🔍 AI, ML, LLM Fundamentals

* **AI vs ML vs LLMs**: Clear distinctions
* **LLM Lifecycle**: Problem -> Dataset -> Model -> Training -> Evaluation -> Deployment
* **Tokenization & Vectorization**: Foundation of how LLMs parse and understand input

### 🔥 AI/LLM Attack Categories

* **Prompt Injection**
* **Jailbreaking & Output Overwriting**
* **Sensitive Information Leakage**
* **Vector Store Attacks & Retrieval Manipulation**
* **Model Weight Poisoning**
* **Data Supply Chain Attacks**

### ⚔️ Prompt Injection Techniques

* "Ignore previous instructions" payloads
* Unicode, emojis, and language-switching evasion
* Markdown/image/HTML-based payloads
* Plugin and multi-modal attack vectors (image, audio, PDF, API)

---

## 🏆 OWASP LLM Top 10 (2024 Version)

| ID    | Risk                           | SEO Keywords                                  |
| ----- | ------------------------------ | --------------------------------------------- |
| LLM01 | Prompt Injection               | "LLM jailbreak", "prompt override"            |
| LLM02 | Sensitive Info Disclosure      | "AI data leak", "PII exfiltration"            |
| LLM03 | Supply Chain Risk              | "dependency poisoning", "model repo hijack"   |
| LLM04 | Data/Model Poisoning           | "AI training corruption", "malicious dataset" |
| LLM05 | Improper Output Handling       | "AI-generated XSS", "model SQLi"              |
| LLM06 | Excessive Agency               | "plugin abuse", "autonomous API misuse"       |
| LLM07 | System Prompt Leakage          | "instruction leakage", "LLM prompt reveal"    |
| LLM08 | Vector Store Vulnerabilities   | "embedding attack", "semantic poisoning"      |
| LLM09 | Misinformation                 | "hallucination", "bias injection"             |
| LLM10 | Unbounded Resource Consumption | "LLM DoS", "token flooding"                   |

➡️ [Read Full OWASP LLM Top 10](https://genai.owasp.org/llm-top-10/)

---

## 🛠️ Offensive AI Pentesting Tools & Frameworks

| Tool                                                                                   | Description                                |
| -------------------------------------------------------------------------------------- | ------------------------------------------ |
| [LLM Attacks](https://llm-attacks.org)                                                 | Directory of adversarial LLM research      |
| [PIPE](https://github.com/jthack/PIPE)                                                 | Prompt Injection Primer for Engineers      |
| [MITRE ATLAS](https://atlas.mitre.org/)                                                | MITRE's AI/ML threat knowledge base        |
| [Awesome GPT Security](https://github.com/cckuailong/awesome-gpt-security)             | Curated LLM threat intelligence tools      |
| [ChatGPT Red Team Ally](https://github.com/NetsecExplained/chatgpt-your-red-team-ally) | ChatGPT usage for red teaming              |
| [Lakera Gandalf](https://gandalf.lakera.ai)                                            | Live prompt injection playground           |
| [AI Immersive Labs](https://prompting.ai.immersivelabs.com/)                           | Prompt attack labs with real-time feedback |
| [AI Goat](https://github.com/dhammon/ai-goat)                                          | OWASP-style AI pentesting playground       |
| [L1B3RT45](https://github.com/elder-plinius/L1B3RT45)                                  | Jailbreak prompt collections               |
| [PromptTrace](https://prompttrace.airedlab.com/)                                       | Interactive AI security training with 7 attack labs, 15-level Gauntlet, and real-time Context Trace for prompt injection and defense bypass |

---

## 💣 Prompt Injection Payload Libraries

* [https://github.com/DummyKitty/Cyber-Security-chatGPT-prompt](https://github.com/DummyKitty/Cyber-Security-chatGPT-prompt)
* [https://github.com/swisskyrepo/PayloadsAllTheThings/tree/master/Prompt%20Injection](https://github.com/swisskyrepo/PayloadsAllTheThings/tree/master/Prompt%20Injection)
* [https://github.com/f/awesome-chatgpt-prompts](https://github.com/f/awesome-chatgpt-prompts)
* [https://gist.github.com/coolaj86/6f4f7b30129b0251f61fa7baaa881516](https://gist.github.com/coolaj86/6f4f7b30129b0251f61fa7baaa881516)

---

## 🧠 Research, Case Studies, and Exploits

### 🔐 Prompt Injection & Jailbreaking

* [https://kai-greshake.de/posts/inject-my-pdf](https://kai-greshake.de/posts/inject-my-pdf)
* [https://www.lakera.ai/blog/guide-to-prompt-injection](https://www.lakera.ai/blog/guide-to-prompt-injection)
* [https://arxiv.org/abs/2306.05499](https://arxiv.org/abs/2306.05499)

### 🧬 Model Poisoning & Supply Chain

* [https://www.csoonline.com/article/3613932/how-data-poisoning-attacks-corrupt-machine-learning-models.html](https://www.csoonline.com/article/3613932/how-data-poisoning-attacks-corrupt-machine-learning-models.html)
* [https://pytorch.org/blog/compromised-nightly-dependency/](https://pytorch.org/blog/compromised-nightly-dependency/)

### 🕷️ Output Handling & Exfil

* [https://systemweakness.com/new-prompt-injection-attack-on-chatgpt-web-version-ef717492c5c2](https://systemweakness.com/new-prompt-injection-attack-on-chatgpt-web-version-ef717492c5c2)

### 🤥 Hallucination, Bias & Ethics

* [https://techpolicy.press/how-should-companies-communicate-the-risks-of-large-language-models-to-users/](https://techpolicy.press/how-should-companies-communicate-the-risks-of-large-language-models-to-users/)

### 🧨 Token Abuse & DoS

* [https://arxiv.org/abs/2006.03463](https://arxiv.org/abs/2006.03463)

---

## 🤝 Contributions Welcome

Want to improve this repo? Here's how:

```bash
# Fork and clone the repo
$ git clone https://github.com/Mr-Infect/AI-penetration-testing
$ cd AI-penetration-testing

# Create a new feature branch
$ git checkout -b feature/my-feature

# Commit, push, and create a pull request
```

---

## 🔍 Keywords 

> `AI Pentesting`, `Prompt Injection`, `LLM Security`, `Mr-Infect AI Hacking`, `ChatGPT Exploits`, `Large Language Model Jailbreak`, `AI Red Team Tools`, `Adversarial AI Attacks`, `OpenAI Prompt Security`, `LLM Ethical Hacking`, `AI Security Github`, `AI Offensive Security`, `LLM OWASP`, `LLM Top 10`, `AI Prompt Vulnerability`, `Token Abuse DoS`, `ChatGPT Jailbreak`, `Red Team AI`, `AI Security Research`

---

## 📞 Contact / Follow

* GitHub Profile: [https://github.com/Mr-Infect](https://github.com/Mr-Infect)
* Project Link: [AI Penetration Testing Repository](https://github.com/Mr-Infect/AI-penetration-testing)

> ⚠️ **Disclaimer**: This project is intended solely for **educational, research, and authorized ethical hacking** purposes. Unauthorized use is illegal.

---

> ⭐️ Star this repository to help others discover top-tier content on AI/LLM penetration testing along with security infra!
