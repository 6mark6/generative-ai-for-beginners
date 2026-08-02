---
mode: agent
description: Create or update a lesson example, assignment, or README in the Generative AI for Beginners curriculum while following repository conventions.
---

# Update a lesson example

You are helping maintain the Generative AI for Beginners curriculum in this workspace.

## Objective
Create or update a lesson example, code sample, or documentation page that is beginner-friendly, self-contained, and consistent with the repository conventions in [AGENTS.md](../../AGENTS.md).

## Inputs
Use the following values when provided:
- Lesson or topic: {{lesson}}
- Target language or format: {{language}} (for example: Python, TypeScript, JavaScript, Markdown, or .NET)
- Desired change: {{change}}
- Relevant files or context: {{context}}

## Repository guidance to follow
- Read [AGENTS.md](../../AGENTS.md) first for project conventions.
- Prefer simple, educational examples over overly complex implementations.
- Keep examples runnable and easy to understand for beginners.
- Use environment variables from .env and .env.copy rather than hardcoded secrets.
- For Azure OpenAI samples, use the Responses API and the /openai/v1/ endpoint.
- For Microsoft Foundry Models, use the appropriate Azure inference client.
- Preserve the repository’s naming and folder conventions.

## Workflow
1. Inspect the relevant lesson directory and related files.
2. Understand the requested change and the surrounding lesson context.
3. Implement the change with the smallest clear edit that satisfies the goal.
4. Update supporting documentation when needed.
5. Validate the result where possible, such as checking syntax, build steps, or markdown consistency.
6. Summarize the changes and any remaining caveats.

## Output format
Provide:
- A short summary of what changed
- The files updated
- Any validation performed
- Any follow-up actions or unresolved issues

## Quality bar
- Keep the tone clear and instructional.
- Avoid unnecessary abstractions.
- Make sure the result is suitable for a beginner learning experience.
