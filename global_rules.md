## Language rules
- When asked questions in a specific language, respond in the same language. All code-related output must remain in English.
- If explicitly requested to translate or generate text in non-English and the file is markdown, proceed. Any text inside code must still be English; this typically applies to source files (e.g., `.py`, `.ts`) rather than markdown.
- Always use English in source code, including:
  - Code comments and documentation
  - User interface messages
  - Error messages and warnings
  - Log messages
  - Debug information
  - Console output
  - Configuration files
  - API responses
  - Status messages
  - Prompts and confirmations

## Code quality
- Always include docstrings for functions and classes.
- Add meaningful comments for complex logic.
- Always use context7 when I need code generation, setup or configuration steps, or library/API documentation. This means you should automatically use the Context7 MCP tools to resolve library id and get library docs without me having to explicitly ask.

## MCP Server Tool usage
- Only call mcp server tools when necessary (e.g., when web search or page fetch is insufficient); avoid calling MCP tools like brave-search and fetch if you already have the needed information.
- When database access is required, proactively use the appropriate MCP server tool based on the requested database type (e.g., Supabase, Oracle, YashanDB, PostgreSQL, etc).

## Git hygiene
- When asked to initializing a repo (`git init`), always create a `.gitignore` at the same time.
- Always add standard recommended items to `.gitignore` based on the project's programming language.

## Git commit message
- Use a clear prefix + subject that reflects the primary changes (e.g., `type(scope): subject` or `type: subject`).
- Keep the subject concise; cover the main modifications, not minor edits.
- In the body, list major change items as bullet points; omit trivial tweaks (e.g., minor wording-only doc edits).
- Describe outcomes/targets of changes, not implementation minutiae.
