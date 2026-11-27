# Changes from the original

Source: the public Remake repository, version 0.1.0, commit `6174ca7`, copied on 27 November 2026.
Licence: MIT. `LICENSE` is kept unchanged, as the licence requires for copies.

Code checked before copying: no analytics, tracking or calls to the original author's servers were found.
The changes below remove every link that tied this copy, or the websites it builds, back to the original author.

| File | Change | Why |
| --- | --- | --- |
| `plugins/remake/skills/remake/SKILL.md` | Installs and updates the engine only from the repo named in your prompt (your own copy), never from the original. Added a rule to move aside any `~/.remake` folder that came from elsewhere. | The original pulled the latest code from the author's repo on every run, so his future changes would run on your computer with your GitHub and Vercel sign-ins. |
| `engine/lib/board.mjs` | Removed the "Made with Remake, by …" footer and its two links. | That footer appeared on the proof page and swap board published on your live site. |
| `engine/lib/ship.mjs` | Removed the "Made with <author's repo>" line from the commit message. | It was written into your own website repo's history. |
| `engine/templates/project/README.md` | Removed the link to the author's repo. | Copied into every website repo you create. |
| `engine/templates/project/package.json` | Removed the author's repo from the description. | Copied into every website repo you create. |
| `engine/lib/util.mjs`, `docs/HOW-IT-WORKS.md` | The browser still says it is "Remake/0.1.0", without the author's repo address. | That address was sent to every website Remake visits. |
| `engine/bin/remake.mjs` | Help text: plain-text credit, no newsletter link. | Promotion link. |
| `package.json`, `.claude-plugin/marketplace.json`, `plugins/remake/.claude-plugin/plugin.json` | Author kept as a plain name; author's website, homepage and repository links removed. | Metadata pointing to the original. |
| `README.md` | Prompts now read `github.com/YOUR-GITHUB-USERNAME/remake`; newsletter, social and subscribe links removed; credits kept as plain names. | So the instructions point to your copy. |

Nothing else was changed. All code files pass a syntax check after the edits.

## Prompt to use with this copy

```text
/goal Remake [LINK] with github.com/YOUR-GITHUB-USERNAME/remake until its report says REMAKE COMPLETE, or stop after 100 turns.
```
