# agent-skills

Agent skills for Claude Code, Codex, and any harness that reads `SKILL.md`.

## resolving-review-comments

Work the comments on an open PR of your own, from human reviewers or review bots (CodeRabbit, Copilot, Qodo).

A review comment is a **claim**, not an instruction. Each one gets one verdict, settled against the code, the spec, or the repo's documented standards:

| Verdict | When |
| --- | --- |
| **Fix** | the claim holds and is in this PR's scope |
| **Reject** | the claim does not hold |
| **Defer** | the claim holds but belongs to other work |
| **Ask** | it cannot be settled without the reviewer |

Verifying a claim is the agent's job; overruling a reviewer is yours, so you see the verdict table before any code moves. Fixes go on top of the reviewed history in themed commits, one push per round, and every comment gets a reply.

The agent reaches for it on its own when a PR comes back with comments, or you can call it by name.

## Install

```bash
npx skills@latest add Hotragn/agent-skills
```

Written in the style of [mattpocock/skills](https://github.com/mattpocock/skills). Not affiliated.

## License

MIT
