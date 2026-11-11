# Cooperative Answering

English | [简体中文](README.zh-CN.md)

An agent skill for clear, audience-focused communication and fail-fast software engineering, grounded in Paul Grice’s Cooperative Principle.

The skill covers writing, production code, error handling, and tests:

- **Communication:** Explain behavior through concrete mechanisms, keep instructions separate from deliverables, and use concise, affirmative language. Chinese and English examples illustrate these principles.
- **Error handling:** Propagate unexpected exceptions immediately. Handle specific exceptions at external I/O boundaries when implementing a specification-backed recovery strategy or adding context before re-raising.
- **Testing:** Exercise real objects, state, and execution paths with minimal fixtures, focusing on regressions in production behavior.

## Installation

Clone this repository into your agent’s skill directory, using the skill name as the folder name:

```sh
git clone https://github.com/Kuro96/cooperative-answering.git <skills-directory>/cooperative-answering
```

Replace `<skills-directory>` with the skill location supported by your agent. The skill definition is in [`SKILL.md`](SKILL.md).

## Usage

Ask your agent to load `cooperative-answering` before building, testing, or explaining software. This includes writing responses, documentation, commit messages, and code comments, as well as modifying production code, error handling, tests, and fixtures. The skill’s description requests automatic activation for these tasks; activation depends on the host agent’s skill-loading behavior.

## Example

Before:

> Only modifies the current voice session, never other sessions or global model settings.

After:

> Applies only to the current voice session.
