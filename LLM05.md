# 🧨 LLM05: Improper Output Handling

Improper Output Handling is one of the most underestimated yet impactful vulnerabilities in LLM-based systems. When LLM-generated outputs are consumed by other applications or directly rendered in web interfaces, failure to properly validate and sanitize these outputs can lead to serious issues like RCE, XSS, SSRF, SQLi, or CSRF.

---

## ⚔️ Exploitation - The Basics

Improper Output Handling typically becomes dangerous when LLMs are connected to downstream systems or applications that automatically trust or execute their responses.

Imagine this:

* You prompt the LLM to summarize some user-submitted HTML.
* The model, being smart (and naive), outputs: `<script>alert('XSS');</script>`.
* If your web app renders that output without sanitization – boom 💥 – a Cross-Site Scripting (XSS) attack just landed.

This isn't just about JavaScript – it could be malformed SQL statements, SSRF payloads, shell commands, or even malicious markdown.

---

## 💻 Sample Exploits & Injection Payloads

### 💥 JavaScript Injection (XSS)

```
Prompt: Summarize this blog post: <script>alert('Hacked!')</script>
```

If the summary is directly rendered on a site without sanitization, the script runs.

### 🧬 SQL Injection

```
Prompt: Suggest a SQL query to fetch user data from a table where username = 'admin'
Output: SELECT * FROM users WHERE username = 'admin' OR '1'='1';
```

If your backend blindly executes LLM output, you're wide open.

### 🧫 Markdown Injection

```
Prompt: Can you show a cool image?
Output: ![Click Me](javascript:alert('XSS'))
```

Rendered in a markdown viewer? That payload just popped.

---

## 🔍 Common Vulnerable Scenarios

* Rendering LLM responses in web frontends.
* Using LLMs to generate code snippets or SQL queries.
* Passing outputs from LLMs directly into shells or command-line scripts.
* Letting LLMs auto-generate markdown, HTML, or JavaScript for preview.

---

## 🔐 How to Mitigate

* **Sanitize Everything**: Run LLM output through sanitization libraries (e.g., DOMPurify for HTML).
* **Context-Aware Escaping**: Use correct escaping based on context (HTML, JS, SQL, etc.).
* **Human-in-the-Loop**: Require manual approval for risky outputs.
* **Rate Limit**: Limit how often certain actions can be performed to reduce DoS risk.
* **Output Filtering**: Block dangerous characters and patterns before rendering/executing.

---

## 📚 Top 15 Deep Dive Resources

1. [PortSwigger Lab - Insecure Output Handling](https://portswigger.net/web-security/llm/insecure-output)
2. [SystemWeakness - Prompt Injection on Web Version](https://systemweakness.com/new-prompt-injection-attack-on-chatgpt-web-version-ef717492c5c2)
3. [OWASP LLM Top 10](https://owasp.org/www-project-top-10-for-large-language-model-applications/)
4. [Snyk - LangChain RCE Vulnerability](https://security.snyk.io/vuln/SNYK-PYTHON-LANGCHAIN-5411357)
5. [ChatGPT Red Team Ally Repo](https://github.com/NetsecExplained/chatgpt-your-red-team-ally)
6. [PayloadsAllTheThings - Prompt Injection](https://github.com/swisskyrepo/PayloadsAllTheThings/tree/master/Prompt%20Injection)
7. [Gandalf Prompt Injection Lab](https://gandalf.lakera.ai)
8. [PIPE - Prompt Injection Primer](https://github.com/jthack/PIPE)
9. [AI Immersive Labs](https://prompting.ai.immersivelabs.com/)
10. [ASCII Smuggler Blog](https://embracethered.com/blog/ascii-smuggler.html)
11. [LangChain Docs - Security Considerations](https://docs.langchain.com/docs/security)
12. [GitHub Gists for Prompt Payloads](https://gist.github.com/coolaj86/6f4f7b30129b0251f61fa7baaa881516)
13. [MITRE ATLAS](https://atlas.mitre.org/)
14. [Awesome GPT Security List](https://github.com/cckuailong/awesome-gpt-security)
15. [OpenAI ChatML Format](https://github.com/openai/openai-python/blob/main/chatml.md)

---

## ✅ Conclusion

Improper Output Handling is a silent killer when integrating LLMs into real-world systems. Always remember: LLMs generate text, not truth, and definitely not safe-by-default output.
