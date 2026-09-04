# Contributing to Awesome LLM Hacking

Thank you for considering contributing to `awesome-llm-hacking`! This repository aims to provide a high-quality, comprehensive, and defense-aware reference for security researchers, red teams, blue teams, and AI developers.

To ensure the list remains curated, high-impact, and accessible, please adhere to the following guidelines before submitting a Pull Request.

---

## 📜 Code of Conduct & Responsible Disclosure

- **Ethical & Defensive Framing:** This repository is intended for research, defensive engineering, and authorized security assessments. Submissions showcasing offensive vectors **must** include defensive context, mitigations, or links to security research.
- **No Zero-Days or Unverified Dumps:** Do **not** submit unverified exploits, active zero-day payloads against production targets, or raw harmful material. 
- **Respect Privacy & Copyright:** Do not link to leaked proprietary model weights, private datasets, or stolen code.

---

## 🛠️ Contribution Guidelines

### 1. Standard Entry Format

All entries must strictly follow this Markdown structure:

```markdown
- [Resource Name](URL) - Concise 1-sentence description ending with a period.
```

#### Formatting Requirements:
- **Resource Name:** The official name of the tool, paper, framework, or CTF (do not include emojis or promotional text in the link label).
- **URL:** Direct hyperlink to the primary source (e.g., GitHub repository, arXiv paper PDF/abstract, official documentation, or security framework).
- **Description:** Exactly **one concise sentence** summarizing what the resource does, how it works, or its security relevance. Ensure correct spelling, punctuation, and grammar.

### 2. Category Taxonomy & Organization

Entries must be categorized under one of the three primary sections:
- **Red Team (Offensive Security):** Direct/Indirect Prompt Injection, Jailbreaking, Model Inversion, Agentic/Tool-Use Exploits, Offensive Scanners.
- **Blue Team (Defensive Mitigations):** Input/Output Guardrails, System Prompt Hardening, Runtime Telemetry/Anomaly Detection, Evaluation Datasets.
- **Purple Team & Practice:** Standards & Threat Models (OWASP, MITRE ATLAS, NIST), CTFs & Sandboxes.

*Note: Maintain alphabetical ordering within each sub-category section.*

### 3. Submission Rules & Quality Criteria

- ❌ **No Spam or Self-Promotion:** Unsolicited marketing, paid affiliate links, or trivial wrappers around generic APIs will be rejected.
- ❌ **No Stale or Abandoned Projects:** Repositories should show active maintenance, clear documentation, or historical research significance.
- ❌ **No Duplicates:** Check existing entries across all sections before submitting a new item.
- ✅ **Dual-Use Awareness:** Offensive tools and datasets should clearly articulate their research or evaluation utility.

---

## 🚀 How to Submit a Pull Request

1. **Fork the Repository:** Create your own copy of `awesome-llm-hacking`.
2. **Create a Feature Branch:** `git checkout -b add/my-awesome-resource`
3. **Add Your Resource:** Place the entry in the correct section in `README.md` following alphabetical order.
4. **Commit Your Changes:** `git commit -m "add: [Resource Name] to [Sub-category]"`
5. **Push & Open PR:** Submit a Pull Request against the `main` branch. Fill out the PR template completely.

Thank you for helping secure the AI ecosystem!
