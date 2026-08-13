I build open-source tools for coding agents, design automation, and the Elixir ecosystem.

I’m interested in the part of AI-assisted development that comes after generation: how an agent inspects what it changed, understands a running system, finds the cause of a failure, and verifies that the result is actually correct.

That has led me to work across design tools, code intelligence, runtimes, build systems, replay, and developer tooling. The projects below approach different parts of the same problem.

## What I’m building now

### Design tools for agents

**[OpenPencil](https://github.com/open-pencil/open-pencil)** is an AI-native, open-source design editor and Figma alternative built with Skia and WebGL. The aim is to make design documents understandable and editable as structured data—not just pixels on a canvas—so both people and agents can inspect and modify them. [Website](https://openpencil.dev)

**[figma-use](https://github.com/dannote/figma-use)** brings that workflow to Figma. It gives agents a CLI for structural queries, JSX rendering, diffs, linting, analysis, patch workflows, exports, and round-tripping. [Show HN](https://news.ycombinator.com/item?id=46665169) · [npm](https://www.npmjs.com/package/figma-use)

### Code intelligence for Elixir

Under **[Elixir Vibe](https://github.com/elixir-vibe)**, I’m building Elixir-native tools that let coding agents work with the structure and runtime of a real codebase instead of treating source files as plain text.

- **[Vibe](https://github.com/elixir-vibe/vibe)** — an experimental BEAM-native coding agent runtime with a TUI, web UI, eval, memory, tools, and subagents.
- **[Reach](https://github.com/elixir-vibe/reach)** — program-dependence graphs, call and data flow, effect analysis, and architecture checks for BEAM projects. [Hex](https://hex.pm/packages/reach)
- **[Exograph](https://github.com/elixir-vibe/exograph)** — structural Elixir code search built with ExAST, Reach, Ecto, and Postgres/ParadeDB. [Hex](https://hex.pm/packages/exograph)
- **[ex_ast](https://github.com/elixir-vibe/ex_ast)** — AST-aware search, replacement, and structural diffs for Elixir. [Hex](https://hex.pm/packages/ex_ast)
- **[ex_dna](https://github.com/elixir-vibe/ex_dna)** — AST-aware duplicate-code detection with extraction candidates. [Hex](https://hex.pm/packages/ex_dna)
- **[ex_slop](https://github.com/elixir-vibe/ex_slop)** — Credo checks for recurring low-quality patterns in generated Elixir code. [Hex](https://hex.pm/packages/ex_slop)
- **[program_facts](https://github.com/elixir-vibe/program_facts)** — generated programs with known structural facts for testing static analyzers. [Hex](https://hex.pm/packages/program_facts)

### Frontend tooling inside the BEAM

**[Elixir Volt](https://github.com/elixir-volt)** explores what Phoenix frontend development looks like when more of the toolchain runs inside the BEAM.

- **[Volt](https://github.com/elixir-volt/volt)** — a frontend build tool and dev server for Phoenix with HMR, Tailwind CSS, and support for JavaScript, TypeScript, Vue, Svelte, React, and Solid. [Hex](https://hex.pm/packages/volt)
- **[Astral](https://github.com/elixir-volt/astral)** — a Volt-powered static site generator for Elixir applications. [Hex](https://hex.pm/packages/astral)
- **[QuickBEAM](https://github.com/elixir-volt/quickbeam)** — a JavaScript runtime for the BEAM with browser-like APIs backed by OTP. [Hex](https://hex.pm/packages/quickbeam) · [Show HN](https://news.ycombinator.com/item?id=47558094)
- **[Phoenix Vapor](https://github.com/elixir-volt/phoenix_vapor)** — Vue templates compiled into native `%Phoenix.LiveView.Rendered{}` structures. [Hex](https://hex.pm/packages/phoenix_vapor)
- **[OXC](https://github.com/elixir-volt/oxc_ex)**, **[Vize](https://github.com/elixir-volt/vize_ex)**, and **[Oxide](https://github.com/elixir-volt/oxide_ex)** — Elixir bindings for JavaScript, Vue, and Tailwind toolchains. [Oxide on Hex](https://hex.pm/packages/oxide_ex)

### Making running systems observable

Static code is only part of the picture. I also work on ways for agents and developers to inspect software while it is running:

- **[pi-elixir](https://github.com/dannote/pi-elixir)** — BEAM runtime tools for the [Pi coding agent](https://github.com/badlogic/pi-mono), including eval, documentation lookup, process state, Ecto queries, logs, and supervisor trees.
- **[phoenix_replay](https://github.com/dannote/phoenix_replay)** — recording and replay for Phoenix LiveView sessions. [Hex](https://hex.pm/packages/phoenix_replay)
- **[live_render](https://github.com/dannote/live_render)** — server-driven generative UI for Phoenix LiveView. [Hex](https://hex.pm/packages/live_render)
- **[phoenix_streamdown](https://github.com/dannote/phoenix_streamdown)** — streaming Markdown for LiveView, designed for incremental LLM output. [Hex](https://hex.pm/packages/phoenix_streamdown)

The larger thesis, architecture, roadmap, and open questions are documented in **[Building Blocks for the Future Web](https://github.com/elixir-vibe/building-blocks)**. It describes how these pieces might fit into a web stack where generated software can be inspected, replayed, traced, and checked.

### Tools I use in my own agent workflow

- **[dot-pi](https://github.com/dannote/dot-pi)** — my extensions, skills, and working rules for Pi.
- **[sloplint](https://github.com/dannote/sloplint)** — an AST-based, multilingual linter for low-quality generated-code patterns.
- **[agentfmt](https://github.com/dannote/agentfmt)** — token-efficient CLI formatting for tools consumed by language models.

## Other open-source work

My current work is mostly around agents and Elixir, but I’ve built open-source software across several ecosystems.

### Phoenix and Elixir libraries

- **[phoenix_spec](https://github.com/dannote/phoenix_spec)** — OpenAPI 3.1 specifications generated from Phoenix JSON views and Ecto schemas. [Hex](https://hex.pm/packages/phoenix_spec)
- **[json_spec](https://github.com/dannote/json_spec)** — Elixir typespec syntax turned into JSON Schema at compile time. [Hex](https://hex.pm/packages/json_spec)
- **[phoenix_iconify](https://github.com/elixir-volt/phoenix_iconify)** and **[iconify](https://github.com/elixir-volt/iconify)** — Iconify SVGs for Elixir, Phoenix, and LiveView. [phoenix_iconify on Hex](https://hex.pm/packages/phoenix_iconify) · [iconify on Hex](https://hex.pm/packages/iconify)
- **[qqr](https://github.com/dannote/qqr)** — a pure-Elixir QR code encoder and decoder. [Hex](https://hex.pm/packages/qqr)

### Ruby

- **[typespec_from_serializers](https://github.com/dannote/typespec_from_serializers)** — TypeSpec descriptions generated from JSON serializers. [RubyGems](https://rubygems.org/gems/typespec_from_serializers)
- **[arel_maniac](https://github.com/dannote/arel_maniac)** — PostgreSQL features for ActiveRecord without raw SQL.

### Search and Russian NLP

- **[Abiko Search](https://github.com/abiko-search)** — a search engine for Tor hidden services, built from scratch in Elixir. It included an Onion v3 implementation and a tor2web proxy. [Product Hunt](https://www.producthunt.com/products/abiko) · [Hacker News](https://news.ycombinator.com/item?id=14927685)
- **[Natasha-Ex](https://github.com/natasha-ex)** — Elixir ports of Russian NLP tools including Yargy, Slovnet, Morph RU, Razmetka, and Razdel.

### Systems and infrastructure

- **[socks-nginx-module](https://github.com/dannote/socks-nginx-module)** — SOCKS5 proxy support for nginx; referenced on the nginx wiki.
- **[lua-template](https://github.com/dannote/lua-template)** — a minimal Lua templating engine adopted by Cloudflare Loom.
- [Desktop-action support for Xfce’s core Garcon library](https://gitlab.xfce.org/xfce/garcon/-/commit/aec77533132eb324180ef771e15226a752573eae) — shipped with Xfce since version 0.6.0.

### Security research

I’ve reported security issues through [Google Bug Hunters](https://bughunters.google.com/profile/62602ae8-cf92-4fb0-810c-c9e284f3427e), [Bugcrowd](https://bugcrowd.com/h/dannote), and the [CodePen bug bounty program](https://bugcrowd.com/engagements/codepen).
