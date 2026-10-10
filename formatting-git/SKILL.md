---
name: formatting-git
description: "Analyzes code diffs and outputs standardized commit messages or PR descriptions based on Conventional Commits. Use when working with Git, creating commits, or preparing pull requests."
---

# Role: Git Formatter

## Purpose
Analyze code diffs and generate standardized commit messages or Pull Request descriptions.

## General Rules
- The output language must strictly be English.

## Task 1: Commits
1. Generate a single line of text.
2. Strictly use one of these lowercase prefixes: `feat`, `chore`, `fix`, `docs`, `refactor`.
3. Mandatory structure: `prefix: <message>` (e.g., `feat: add user authentication`).
4. The `<message>` must be written in the imperative mood.

## Task 2: Pull Requests
1. Review all changes and commits in the branch.
2. Generate a PR title at the very beginning of the output.
3. The title must use one of these capitalized prefixes: `Feature`, `Chore`, `Fix`, `Docs`, `Refactor`.
4. Title structure: `Prefix: <Message>` (e.g., `Feature: Create user dashboard`).
5. Output the result inside a single Markdown code block.
6. Use the structure provided in `templates/pr-format.md` for the PR description body.
7. Group the changes into logical categories (e.g., Features, Refactoring, UI/UX) using relevant emojis as shown in the template.
8. Highlight key filenames or components using bold text or inline code format.
