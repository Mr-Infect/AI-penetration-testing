# 🛡️ AI/ML/LLM Penetration Testing Resources

Welcome to the **AI/ML/LLM Penetration Testing Resources** repository!

This collection offers a **comprehensive set of tools, articles, labs, and references** to help understand, identify, and mitigate vulnerabilities in **Artificial Intelligence (AI)**, **Machine Learning (ML)**, and **Large Language Models (LLMs)**.

Whether you're a cybersecurity professional or just diving into the world of AI security, this repo is designed to equip you with **hands-on knowledge and practical tools** for pentesting AI-powered systems.

---

## 🌟 Why is AI/ML/LLM Pentesting Important?

As AI becomes embedded into healthcare, finance, law, and beyond, securing these models is more crucial than ever. Vulnerabilities in AI/LLM systems can lead to:

- 🕵️ Sensitive Information Disclosure  
- 🤖 Malicious Model Behavior (bias, hallucinations, offensive outputs)  
- 🚫 Service Disruption (DoS attacks)  
- 📦 Intellectual Property Theft  
- 🛠️ Supply Chain Compromises  

This repository helps you address these risks by learning how to break (ethically) and fix these systems.

---

## 🚀 Getting Started

To get the most from this repository, basic knowledge in the following areas is helpful:

- 🔬 AI & ML Concepts (model training, data pipelines)
- 🧠 Large Language Models (architecture & applications)
- 🧑‍💻 Traditional Pentesting (XSS, SQLi, API security)
- 🐍 Python Programming (most tools/scripts are Python-based)

---

## 📚 Resources Overview

### 💡 AI/LLM Introduction & Fundamentals

- **What is AI?**  
  Machines simulating human intelligence (learning, reasoning, problem-solving).

- **Language Models & LLMs**  
  Models that understand and generate human language (e.g., ChatGPT, Claude).

- **Training LLMs**  
  Using massive text datasets to learn syntax, meaning, and knowledge.

- **Development Lifecycle**  
  `Problem → Data Collection → Model Design → Training → Evaluation → Deployment → Monitoring`

- **Tokenization**  
  Breaking text into machine-readable units (tokens).

---

## 🚨 AI/LLM Attack Landscape

### 🔥 Core Attack Categories

- **Misalignment**: Offensive outputs, hallucinations, bias  
- **Jailbreaks**: Prompt overwriting, system instruction manipulation  
- **Prompt Injections**: Exfiltration, plugin abuse, instruction overriding  

### 🧪 Injection Techniques

- “Ignore previous instructions”  
- Obfuscation with emojis, encoding, or switching languages  
- Exploiting plugin capabilities (email, web browsing, API calls)  
- Markdown image/data exfiltration  
- Injection across multiple file formats (text, image, audio, video)

---

## ⚔️ OWASP Top 10 for LLM Applications

Adapted from OWASP's LLM Top 10 framework:

| ID | Title | Description |
|----|-------|-------------|
| **LLM01** | Prompt Injection | Trick models into revealing secrets, bypassing instructions |
| **LLM02** | Sensitive Information Disclosure | Accidental leakage of PII, financial data |
| **LLM03** | Supply Chain | Risk from external components or poisoned datasets |
| **LLM04** | Data / Model Poisoning | Malicious manipulation of training data or weights |
| **LLM05** | Improper Output Handling | LLM-generated XSS, SQLi, RCE |
| **LLM06** | Excessive Agency | Unchecked plugin/API interaction causing harm |
| **LLM07** | System Prompt Leakage | Leaking internal system instructions or secrets |
| **LLM08** | Vector & Embedding Weaknesses | Attacks via vector stores & embeddings |
| **LLM09** | Misinformation | Hallucinated or biased outputs causing harm |
| **LLM10** | Unbounded Consumption | Abuse via DoS or unauthorized model replication |

👉 **[Read the full OWASP LLM Top 10](https://genai.owasp.org/llm-top-10/)**

---

## 🛠️ Tools & Frameworks

| Name | Description |
|------|-------------|
| [LLM Attacks](https://llm-attacks.org) | Adversarial LLM security research |
| [PIPE](https://github.com/jthack/PIPE) | Prompt Injection Primer for Engineers |
| [MITRE ATLAS](https://atlas.mitre.org/) | AI/ML threat techniques database |
| [Awesome GPT Security](https://github.com/cckuailong/awesome-gpt-security) | Curated GPT security list |
| [ChatGPT Red Team Ally](https://github.com/NetsecExplained/chatgpt-your-red-team-ally) | Using ChatGPT in red teaming |
| [Lakera Gandalf](https://gandalf.lakera.ai) | Prompt injection lab playground |
| [AI Immersive Labs](https://prompting.ai.immersivelabs.com/) | Hands-on labs for prompt attacks |
| [AI Goat](https://github.com/dhammon/ai-goat) | Research playground for AI security |
| [L1B3RT45](https://github.com/elder-plinius/L1B3RT45) | List of known LLM jailbreaks |

---

## 🧰 Prompt Injection Payload Collections

- https://github.com/DummyKitty/Cyber-Security-chatGPT-prompt  
- https://github.com/swisskyrepo/PayloadsAllTheThings/tree/master/Prompt%20Injection  
- https://github.com/f/awesome-chatgpt-prompts  
- https://gist.github.com/coolaj86/6f4f7b30129b0251f61fa7baaa881516  

---

## 📄 Articles & Research

### 🧠 Prompt Injection
- https://kai-greshake.de/posts/inject-my-pdf  
- https://www.lakera.ai/blog/guide-to-prompt-injection  
- https://arxiv.org/abs/2306.05499

### 🔐 Sensitive Info Disclosure
- https://cybernews.com/security/chatgpt-samsung-leak-explained-lessons/

### 🧪 Supply Chain Attacks
- https://pytorch.org/blog/compromised-nightly-dependency/

### ☣️ Model Poisoning
- https://www.csoonline.com/article/3613932/how-data-poisoning-attacks-corrupt-machine-learning-models.html

### 🕷️ Improper Output Handling
- https://systemweakness.com/new-prompt-injection-attack-on-chatgpt-web-version-ef717492c5c2

### 🤥 Misinformation & Hallucinations
- https://techpolicy.press/how-should-companies-communicate-the-risks-of-large-language-models-to-users/

### 💥 Unbounded Consumption
- https://arxiv.org/abs/2006.03463

---

## 🤝 Contributing

Contributions are what make the open-source world amazing!  
If you have new tools, fixes, or better explanations:

1. Fork the project  
2. Create a new branch: `git checkout -b feature/AmazingFeature`  
3. Commit changes: `git commit -m 'Add some AmazingFeature'`  
4. Push: `git push origin feature/AmazingFeature`  
5. Submit a pull request 🎉

---

## 📄 License

Distributed under the **MIT License**.  
See `LICENSE` file for more details.

---

## 📞 Contact
 
**Project Link:** [https://github.com/Mr-Infect/AI-penetration-testing](https://github.com/Mr-Infect/AI-penetration-testing)

---

> ⚠️ **Disclaimer:** This repository is for **educational and ethical hacking** purposes only. Do not use these tools without explicit permission. Unauthorized testing is illegal and unethical.
