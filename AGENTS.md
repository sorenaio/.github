# AGENTS.md - .github

This is the agent instruction file for this repository; `CLAUDE.md` is a symlink to it.

## Subagents

- Parallel by default: launch every independent subtask as a parallel Sonnet subagent in one message; go sequential only when a step needs another's result, and never wait on work that could already be running.
- Give heavy or long work to Sonnet subagents: implementing tasks, research or info gathering that needs a lot of reading, and long-running checks or polling that would otherwise burn tokens in the main context.
