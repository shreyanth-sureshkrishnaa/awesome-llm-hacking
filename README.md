# Awesome LLM Hacking

> A curated, defense-aware list of offensive security techniques (Red Team), defensive mitigations (Blue Team), and dual-use benchmarks/tooling (Purple Team) for Large Language Models (LLMs) and Generative AI applications.

This repository serves as an educational and technical resource for security researchers, AI red teams, defensive engineers, and AI developers working to understand and mitigate security risks associated with Large Language Models and agentic systems.

---

## Table of Contents

- [Red Team (Offensive Security)](#red-team-offensive-security)
  - [Direct & Indirect Prompt Injection](#direct--indirect-prompt-injection)
  - [Jailbreaking & Alignment Breaking](#jailbreaking--alignment-breaking)
  - [Model Inversion & Training Data Extraction](#model-inversion--training-data-extraction)
  - [Agentic & Tool-Use Exploits](#agentic--tool-use-exploits)
  - [Offensive Security Frameworks & Automated Scanners](#offensive-security-frameworks--automated-scanners)
- [Blue Team (Defensive Mitigations)](#blue-team-defensive-mitigations)
  - [Input/Output Guardrails & Filtering Frameworks](#inputoutput-guardrails--filtering-frameworks)
  - [System Prompt Hardening & Architecture](#system-prompt-hardening--architecture)
  - [Runtime Anomaly Detection & Telemetry](#runtime-anomaly-detection--telemetry)
  - [Model Safety Evaluation Datasets](#model-safety-evaluation-datasets)
- [Purple Team / Practice](#purple-team--practice)
  - [Security Standards & Threat Models](#security-standards--threat-models)
  - [Interactive CTFs & Vulnerable LLM Sandboxes](#interactive-ctfs--vulnerable-llm-sandboxes)
- [Contributing](#contributing)
- [License](#license)

---

## Red Team (Offensive Security)

### Direct & Indirect Prompt Injection

- [BIPIA Benchmark](https://github.com/microsoft/BIPIA) - A benchmark dataset for evaluating model robustness against indirect prompt injection attacks in text processing tasks.
- [Ignore This Title: Indirect Prompt Injection Attacks on LLMs](https://arxiv.org/abs/2302.12173) - Fundamental paper by Greshake et al. demonstrating how untrusted content in retrieval pipelines can subvert system instructions.
- [Injected Prompt Security Benchmark (SecLists Prompt Injection)](https://github.com/danielmiessler/SecLists) - Collection of payload patterns and prompt injection sequences for automated vulnerability testing.
- [Not What You’ve Signed Up For: Compromising Real-World LLM Applications via Indirect Prompt Injection](https://arxiv.org/abs/2302.12173) - Comprehensive security analysis on data exfiltration and control hijacking in interconnected LLM agents.
- [Prompt Injection Attack Vectors (Perez & Ribeiro)](https://arxiv.org/abs/2208.05309) - Early foundational paper defining direct prompt injection, goal hijacking, and prompt leaking techniques.

### Jailbreaking & Alignment Breaking

- [AdvGLUE](https://advglue.github.io/) - A multi-task adversarial benchmark assessing model stability under textual perturbations and adversarial prompts.
- [AutoDAN: Generating Stealthy Jailbreak Prompts Automatically](https://arxiv.org/abs/2310.04451) - An automated gradient-based and genetic jailbreak generator producing fluent adversarial prompts.
- [Do-Not-Answer Dataset](https://github.com/LibrAI/do-not-answer) - An open dataset of safety-critical prompts designed to evaluate safety alignment across sensitive categories.
- [JailbreakEval](https://github.com/beaver-dam/jailbreak-eval) - A standardized framework for assessing the effectiveness and success rate of adversarial jailbreak attacks.
- [Many-Shot Jailbreaking](https://www.anthropic.com/research/many-shot-jailbreaking) - Anthropic research detailing how long-context windows enable alignment overrides through repeated in-context examples.
- [PAIR (Prompt Automatic Iterative Refinement)](https://arxiv.org/abs/2309.10253) - An algorithm using an attacker LLM to automatically engineer targeted jailbreaks against a defender LLM without gradient access.
- [TAP (Tree of Attacks with Pruning)](https://arxiv.org/abs/2312.02119) - An automated black-box jailbreaking framework utilizing tree search and pruning to efficiently bypass safety filters.
- [Universal and Transferable Adversarial Attacks on Aligned Language Models (GCG)](https://arxiv.org/abs/2307.15043) - Zou et al. introducing Greedy Coordinate Gradient suffix optimization to generate transferable jailbreak tokens.

### Model Inversion & Training Data Extraction

- [AI Privacy Meter](https://github.com/privacytrustlab/privacy-meter) - Tool for quantitative evaluation of privacy risks and membership inference vulnerabilities in machine learning models.
- [Extracting Training Data from Large Language Models](https://arxiv.org/abs/2012.07805) - Landmark paper by Carlini et al. demonstrating verbatim extraction of private training data from generative models.
- [Membership Inference Attacks against Language Models](https://arxiv.org/abs/2205.10962) - Empirical study evaluating privacy leakage and membership detection in fine-tuned and pre-trained LLMs.
- [Scalable Extraction of Training Data from Production LLMs](https://arxiv.org/abs/2311.17035) - Nasr et al. demonstrating practical data extraction techniques against commercial production alignment guardrails.
- [The Secret Sharer: Evaluating and Testing Unintended Memorization in Neural Networks](https://arxiv.org/abs/1802.08232) - Methodology for measuring unintended memorization of sensitive tokens in language models.

### Agentic & Tool-Use Exploits

- [CVE-2023-36258 (LangChain RCE)](https://nvd.nist.gov/vuln/detail/CVE-2023-36258) - Vulnerability analysis of arbitrary code execution vectors arising from unsafe experimental tool evaluation in LangChain.
- [PoisonedRAG: Knowledge Corruption Attacks on Retrieval-Augmented Generation](https://arxiv.org/abs/2402.07867) - Research introducing targeted knowledge poisoning attacks against RAG vector stores to manipulate downstream responses.
- [Spilling the Beans: Privilege Escalation in Agentic Tool Calls](https://arxiv.org/abs/2403.02691) - Study analyzing tool authorization vulnerabilities and cross-domain privilege escalation in autonomous LLM agents.
- [SSRF in Web-Browsing AI Plugins](https://portswigger.net/web-security/llm) - Exploitation methodology demonstrating Server-Side Request Forgery via unvalidated fetch commands issued by LLM web tools.
- [Universal Vulnerabilities in Agentic Systems](https://arxiv.org/abs/2401.12345) - Taxonomy and breakdown of security failures in multi-agent orchestration frameworks and tool calling APIs.

### Offensive Security Frameworks & Automated Scanners

- [Adversarial Robustness Toolbox (ART)](https://github.com/Trusted-AI/adversarial-robustness-toolbox) - IBM library providing developer tools for evaluating and hardening models against adversarial attacks.
- [Garak](https://github.com/leondz/garak) - The Generative AI Red-Teaming & Assessment Kicker for scanning LLMs for prompt injection, jailbreaks, and hallucinations.
- [Inspect](https://github.com/UKGovernmentBEIS/inspect_ai) - Framework built by the AI Safety Institute for evaluation of AI model capabilities and safety boundaries.
- [Promptfoo](https://github.com/promptfoo/promptfoo) - CLI tool and framework for testing LLM app security, prompt injections, output quality, and guardrail bypasses.
- [PyRIT (Python Risk Identification Tool for AI)](https://github.com/Azure/PyRIT) - Microsoft framework enabling red teams to automate security assessments and risk identification in GenAI applications.

---

## Blue Team (Defensive Mitigations)

### Input/Output Guardrails & Filtering Frameworks

- [Azure AI Content Safety](https://learn.microsoft.com/en-us/azure/ai-services/content-safety/) - Enterprise API service detecting prompt injections, unsafe content, and multi-modal risk vectors.
- [Guardrails AI](https://github.com/guardrails-ai/guardrails) - Framework for specifying semantic validation rules and enforcing output structure, safety policies, and schema constraints.
- [Lakera Guard](https://www.lakera.ai/) - Commercial and API-based real-time security boundary defending against prompt injection and data exfiltration.
- [Llama Guard 3 & Prompt Guard](https://github.com/meta-llama/llama-models) - Meta open-weight foundation models specifically fine-tuned for input/output safety classification and injection filtering.
- [LLM Guard (Protect AI)](https://github.com/protectai/llm-guard) - Toolkit designed to sanitize LLM inputs and outputs against prompt injection, PII leakage, and malicious code.
- [NeMo Guardrails](https://github.com/NVIDIA/NeMo-Guardrails) - NVIDIA toolkit for adding programmable guardrails using Colang to control LLM dialogue flow and safety parameters.

### System Prompt Hardening & Architecture

- [Dual-LLM Security Pattern](https://simonwillison.net/2023/Apr/25/dual-llm-pattern/) - Architectural design pattern separating untrusted data processing (unprivileged model) from decision execution (privileged model).
- [Instruction Hierarchy (OpenAI Research)](https://arxiv.org/abs/2404.13208) - Defensive framework for training models to prioritize privileged system instructions over unprivileged user or third-party context.
- [Prompt Sandwich & Delimiter Framing](https://learn.promptingguide.ai/risks/adversarial#prompt-sandwich) - Engineering technique wrapping untrusted inputs between rigid system boundary tokens to enforce instruction scope.
- [Structural XML/JSON Output Enforcement](https://docs.anthropic.com/en/docs/build-with-claude/prompt-engineering/use-xml-tags) - Best practice guide utilizing structured schema delimiters to isolate operational instructions from payload data.

### Runtime Anomaly Detection & Telemetry

- [Arize Phoenix](https://github.com/arize-ai/phoenix) - Open-source AI observability platform for tracing LLM execution, monitoring embedding drifts, and analyzing agentic tool calls.
- [HoneyTokens in RAG Vector Databases](https://www.canarytokens.org) - Defensive deployment strategy placing canary data points in vector stores to alert on unauthorized retrieval or exfiltration attempts.
- [LangSmith](https://www.langchain.com/langsmith) - Observability and monitoring suite providing end-to-end trace logging for detecting runtime prompt injection and anomalous chain execution.
- [Latent Space & Logit Perplexity Monitoring](https://arxiv.org/abs/2308.09348) - Research methodology leveraging output token distribution perplexity and latent representation anomalies to flag injection attacks.
- [OpenInference / OpenTelemetry GenAI](https://github.com/Arize-ai/openinference) - Open standard semantic conventions for instrumenting GenAI application traces and security telemetry.

### Model Safety Evaluation Datasets

- [BeaverTails](https://github.com/PKU-Alignment/BeaverTails) - Safety alignment dataset providing human annotations for safety bounds and red-teaming prompt evaluation.
- [DecodingTrust](https://decodingtrust.github.io/) - Comprehensive benchmark for evaluating trustworthiness, toxicity, bias, privacy, and robustness in LLMs.
- [HarmBench](https://github.com/centerforaisafety/HarmBench) - Standardized evaluation framework for automated red-teaming and safety validation across open and closed models.
- [XSTest (Exaggerated Safety Test)](https://github.com/edwardjhu/xstest) - Test suite designed to measure false-positive refusals and exaggerated safety behaviors in aligned LLMs.

---

## Purple Team / Practice

### Security Standards & Threat Models

- [ISO/IEC 42001 AI Management System](https://www.iso.org/standard/81230.html) - International standard specifying requirements for establishing, implementing, and continually improving an AI management system.
- [MITRE ATLAS (Adversarial Threat Landscape for AI Systems)](https://atlas.mitre.org/) - Knowledge base of adversary tactics, techniques, and case studies targeting AI-enabled systems.
- [NIST AI Risk Management Framework (AI RMF 1.0)](https://www.nist.gov/itl/ai-risk-management-framework) - Federal guideline for managing risks to individuals, organizations, and society associated with artificial intelligence.
- [NIST SP 800-218A (Secure Software Development for GenAI)](https://csrc.nist.gov/) - Special publication detailing secure lifecycle controls for generative AI and LLM software integrations.
- [OWASP Top 10 for Large Language Model Applications](https://owasp.org/www-project-top-10-for-large-language-model-applications/) - Industry standard classification of the top critical security vulnerabilities present in LLM applications.

### Interactive CTFs & Vulnerable LLM Sandboxes

- [Double-Cross CTF](https://github.com/prompthacking/ctf) - Interactive prompt injection challenges focused on extraction of hidden system flags and bypass of input filters.
- [Gandalf by Lakera](https://gandalf.lakera.ai/) - Multi-level interactive LLM security challenge testing prompt injection and alignment extraction techniques.
- [HackAPrompt Benchmark & CTF](https://github.com/HackAPrompt/HackAPrompt) - Competition and dataset evaluating prompt hacking techniques across hundreds of thousands of user submissions.
- [OWASP Juice Shop GenAI Extension](https://owasp.org/www-project-juice-shop/) - Intentionally vulnerable web application incorporating GenAI vulnerabilities, tool abuse, and prompt injection labs.
- [PortSwigger Web Security Academy: LLM Attacks](https://portswigger.net/web-security/llm) - Interactive hands-on labs covering indirect prompt injection, tool hijacking, and remote code execution vulnerabilities.

---

## Contributing

Contributions are welcome! Please read the [Contributing Guidelines](CONTRIBUTING.md) and review the [Pull Request Template](.github/PULL_REQUEST_TEMPLATE.md) before submitting an entry.
