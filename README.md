# Cooperative Answering

An agent skill for clear, concise, audience-focused communication, grounded in Paul Grice’s Cooperative Principle.

The skill guides agents to explain behavior through concrete mechanisms, keep instructions separate from deliverables, and remove redundant or defensive phrasing. It includes Chinese and English examples for explanations, documentation, code comments, and completion reports.

## Installation

Clone this repository into your agent’s skill directory, using the skill name as the folder name:

```sh
git clone https://github.com/Kuro96/cooperative-answering.git <skills-directory>/cooperative-answer
```

Replace `<skills-directory>` with the skill location supported by your agent. The skill definition is in [`SKILL.md`](SKILL.md).

## Usage

Ask your agent to load `cooperative-answer` before writing a response or document. The skill’s description requests automatic activation for user-facing writing; activation depends on the host agent’s skill-loading behavior.

## Example

Before:

> Only modifies the current voice session, never other sessions or global model settings.

After:

> Applies only to the current voice session.
