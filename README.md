# Reproducing and extending Schelling's segregation model with an AI agent

Eric Gladstone · research walkthrough · independent work · October 2026.

A recorded Claude Code session, presented as it was worked through. The Claude Code console is on the left and the commentary is on the right. Starting from a brief based on published descriptions of Thomas Schelling's checkerboard model, the session specifies the model, fixes measures and pass criteria before running, tests the code against cases with known answers, attempts the reproduction, varies the choices the description leaves open, and extends two assumptions the original holds fixed: exact perception of one's neighborhood, and neighborhoods defined by adjacency. The 8×8 demonstration fails its predetermined test. The general relationship reproduces on 40×40 boards.

- **Live:** https://agentbasedmodel.eric-c-gladstone.workers.dev
- **Also at:** https://graystoneindustries.co/talks/#agent-based-model (embedded)

## What is verbatim and what is editorial

Claude's replies and tool output are verbatim, from one continuous session (Claude Code 2.1.294, Opus 5.5), recorded 9 October 2026. The brief and the 13 questions were prepared in a separate AI-assisted planning session. Turn 7 was restarted with a revised question after turn 6 reported a failed pre-specified test: the first attempt was stopped before it produced any output or touched any file, and the session continued from the exact end of turn 6. Timing, grouping into parts, focus, and the commentary on the right are editorial.

The session worked from later descriptions of the model, not the original texts. Its brief differs from Schelling (1978, pp. 148–149) in the 8×8 perturbation and in leaving the destination rule open, as the walkthrough states.

## Use

Open it and step with ← →. Use shift+← → to move between sections and space to play. A− / A+ (or the - and = keys) change the terminal text size. URL options: `?s=<screen>&b=<part>` opens at a given point, `?play=1` autoplays, `?t=<px>` sets the terminal size, and `?embed=1` fills its frame for embedding.

Run locally with any static server, for example `python3 -m http.server 4751 --directory public`.

## Files

`public/` is the whole site: `index.html`, `app.js`, `style.css`, `data/session.js` (the session, as the page plays it), `data/walkthrough.js` (the commentary), self-hosted Geist fonts, and `vendor/marked.umd.js` (MIT) for rendering Markdown. It makes no third-party requests.

## Reference

Schelling, T. C. (1971). Dynamic models of segregation. *Journal of Mathematical Sociology*, 1(2), 143–186.
Schelling, T. C. (1978). *Micromotives and macrobehavior*. W. W. Norton & Company.
