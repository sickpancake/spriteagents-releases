# SpriteAgents

An agentic development environment (ADE) designed to make running coding agents something you
can actually see.

Coding agents work invisibly, off in terminal tabs, and the more of them you run the more time
you spend checking which one is stuck, which one needs you, and which one finished ten minutes
ago. SpriteAgents gives them a pixel-art office instead. Every agent gets a desk and a sprite,
and the one that needs you looks like it needs you.

Works with Claude Code, Codex, and Opencode.

**Status: pre-alpha (v0.1.0).** Free to use. macOS only for now.

This repository exists to host the downloads. The source isn't public yet.

## Install

Easiest from the terminal, which also skips a macOS security warning:

```bash
curl -L -o /tmp/SpriteAgents.zip \
  https://github.com/sickpancake/spriteagents-releases/releases/latest/download/SpriteAgents-mac-arm64.zip
unzip -q /tmp/SpriteAgents.zip -d /Applications
```

Use `SpriteAgents-mac-x64.zip` on an Intel Mac. (Apple menu, then About This Mac. If it says
"Apple M" anything, you want Apple Silicon.)

Prefer clicking? There are `.dmg` files on the
[Releases page](https://github.com/sickpancake/spriteagents-releases/releases/latest), but they
need one extra step. These builds aren't signed yet, and macOS only bothers checking files that
arrived through a browser, which is why the terminal route above avoids the whole thing. Drag
the app into Applications, then run:

```bash
xattr -d com.apple.quarantine /Applications/SpriteAgents.app
```

## What works

* Start a Claude Code, Codex, or Opencode sprite in whatever folder you're working in, and type
  into its terminal from the app.
* Keep several projects open and flip between them. Each folder gets its own office, the ones
  you aren't watching keep running, and your layout is saved per project.
* Close a terminal and come back to it later with its scrollback intact.
* Quit the app without killing anything. The agents keep running.
* Eight desks. A ninth agent waits for a seat rather than disappearing.

Everything runs on your machine. No account, no telemetry, nothing uploaded.

## What's missing

* macOS only. Windows and Linux are planned.
* Builds aren't signed yet.
* You still approve permission prompts in the terminal, not the office.
* No cost tracking, transcript browser, or diff review.
* No agent-to-agent messaging and no shared memory. Those are the point of the project and
  they come next.

## License

Free to download and use. All rights reserved for now, so no copying, modifying, or
redistributing. Open-sourcing is on the table once the project has some traction.

Mascot art shows you which agent is which, nothing more, and belongs to its respective owners.
