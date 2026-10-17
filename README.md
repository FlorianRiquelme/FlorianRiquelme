# Florian Riquelme

Senior software engineer at SVO Netz GmbH in Celle, part of SVO-Gruppe, a regional energy and infrastructure provider. I turn team prototypes into production software, and I look after the group's customer websites.

I work AI-first. Coding agents do most of the typing. I set the guardrails, review the output, and own what ends up in production.

## Featured

**[friquelme.dev](https://github.com/FlorianRiquelme/friquelme.dev)**: My personal site and blog, built entirely by coding agents. Astro on AWS (S3, CloudFront, CDK), deployed by GitHub Actions through OIDC. The interesting part is the delivery pipeline around it:

- Every PR gets an independent review from a separate agent with fresh context. That agent checks the tests by mutating the code they claim to cover.
- The verdict is posted as a structured comment that a required status check reads. No PASS for the exact head commit means no merge.
- Agents merge only through a merge guard. It refuses unless both verification gates passed on that head in a clean tree, and unless every bot review thread has an answer.
- After a deploy, a smoke test checks production. If it fails, the last good build goes back up automatically and an incident issue gets opened.

More on how this works is coming soon.

**[screengrab](https://github.com/FlorianRiquelme/screengrab)**: Screenshot to AI agent in three keystrokes. A macOS menu bar app that puts the screenshot's file path on your clipboard so Claude Code, Codex or any other agent can read it. Swift, runs entirely on your Mac. v1.0.0 is out.

```
brew install --cask FlorianRiquelme/tap/screengrab
```

## Agent tooling

- [claudefuel](https://github.com/FlorianRiquelme/claudefuel): A fuel gauge for Claude Code. A status bar for context usage, rate limits and reset times that knows about multiple accounts.
- [openrouter-zdr](https://github.com/FlorianRiquelme/openrouter-zdr): An OpenRouter client that only routes to zero-data-retention endpoints, with no option to turn that off.
- [jev-kit](https://github.com/FlorianRiquelme/jev-kit): A typed client and benchmark harness for TypeSafe AI's Jev decision model. It measures accuracy, calibration and cost on your own data before you trust a threshold.

## Writing

I write about working with AI in real codebases at [friquelme.dev](https://friquelme.dev).

- [designing for the operator](https://friquelme.dev/blog/designing-for-the-operator/) (May 2026)

## Stack

PHP, Laravel, Statamic, TypeScript, Go, Swift, AWS (CDK, Terraform). I work in Claude Code, Codex and Cursor.

## Contact

[friquelme.dev](https://friquelme.dev) · [flo@friquelme.dev](mailto:flo@friquelme.dev) · [LinkedIn](https://www.linkedin.com/in/florian-riquelme-b97756143)
