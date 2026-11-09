# Koala Canvas

A local canvas for proofs of concept. An agent lays out live variants of any web project side by side, in rounds (layout, then visual). You mark each one Pick, Maybe or Out, pin comments, ask for more or a mix, and choose. The decision is recorded and the losing options freeze into images.

Everything runs on your machine. Frames are live routes of your own dev server, and state lives in `.koala-canvas/` in your project.

This repo holds the installable package only. The source is private.

## Install

Needs Node 20 or later.

```bash
npm i -g https://github.com/jespinosa19/koala-canvas-releases/releases/latest/download/koala-canvas.tgz
koala-canvas skill
```

`koala-canvas skill` installs the agent skill in `~/.claude/skills/koala-canvas`, so Claude Code knows how to use the canvas in any project.

## Use

Start your project's dev server, then from the project root:

```bash
koala-canvas serve --target http://localhost:3000
```

Open `http://localhost:4848/__canvas/` and ask your agent to put options on the canvas. Add `.koala-canvas/` to your `.gitignore`.

`koala-canvas screenshot` and `decide` need Chrome or Chromium (`CHROME_PATH` if it is not on the PATH).

## Update

Run the install command again.

More: https://www.jordiespinosa.com/projects/koala-canvas
