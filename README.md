# 🧠 Agent Skills

This repository contains a collection of skills (tools, context rules, and workflows) designed to standardize AI agent behaviors in environments like Antigravity IDE, OpenCode, and Codex.

## 📚 Skills Catalog

| Skill | Description | Status |
| :---- | :---------- | :----- |


## ⚙️ Modular Architecture

Each skill is self-contained within its own directory using the following structure:
- `skill.yaml`: Metadata and execution triggers for the IDE engine.
- `SKILL.md`: Semantic instructions, constraints, and roles for the LLM.
- `templates/` (Optional): Base templates, scripts, or reference resources.

## 🚀 Installation & Usage

**Global Configuration (Recommended):**
Clone this repository into your local directory and point your IDE's global skills configuration to this path:
```bash
git clone https://github.com/brytekatze/skills.git ~/.agent-skills
```

**Per-Project Configuration (Submodules):**
To bind these rules to a specific project (e.g., SiftFiles), add it as a submodule:
```bash
git submodule add https://github.com/brytekatze/skills.git .skills
