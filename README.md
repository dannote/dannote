I build tools for agents that work with code, design, and running systems.

Agents can generate changes quickly, but they still need good feedback to verify the result. My work exposes structure around software artifacts — design trees, visual diffs, code ASTs, runtime state, build graphs, checks, replay, and feedback loops — so agents can inspect, modify, and correct their work more reliably.

## Current work

### Design tooling

**[OpenPencil](https://github.com/open-pencil/open-pencil)** — AI-native design editor and open-source Figma alternative built on Skia/WebGL. [Website](https://openpencil.dev)

**[figma-use](https://github.com/dannote/figma-use)** — Agent-facing Figma CLI with JSX rendering, structural queries, diffs, linting, analysis, patch workflows, export, and round-tripping. [Show HN](https://news.ycombinator.com/item?id=46665169) · [npm](https://www.npmjs.com/package/figma-use)

### Coding agents and code intelligence

**[Elixir Vibe](https://github.com/elixir-vibe)** — Elixir-native tooling for agent-assisted coding: AST-aware edits, duplicate detection, generated-code checks, program-dependence graphs, structural code search, and a BEAM-native agent runtime.

Projects:

- **[Vibe](https://github.com/elixir-vibe/vibe)** — experimental BEAM-native coding agent runtime with TUI, web UI, eval, memory, tools, and subagents.
- **[Reach](https://github.com/elixir-vibe/reach)** — program dependence graph, call/data-flow, architecture checks, and effect analysis for BEAM projects.
- **[Exograph](https://github.com/elixir-vibe/exograph)** — structural Elixir code search powered by ExAST, Reach, Ecto, and Postgres/ParadeDB.
- **[ex_ast](https://github.com/elixir-vibe/ex_ast)** — AST-aware search, replace, and diffs for Elixir code. [Hex](https://hex.pm/packages/ex_ast)
- **[ex_dna](https://github.com/elixir-vibe/ex_dna)** — AST-aware duplicate-code detection with extraction candidates. [Hex](https://hex.pm/packages/ex_dna)
- **[ex_slop](https://github.com/elixir-vibe/ex_slop)** — Credo checks for low-quality AI-generated Elixir patterns.
- **[program_facts](https://github.com/elixir-vibe/program_facts)** — generated Elixir programs with known structural facts for analyzer testing.

### Frontend runtime and build tooling

**[Elixir Volt](https://github.com/elixir-volt)** — frontend tooling for Phoenix that runs inside the BEAM: JS/TS/Vue/Tailwind builds, HMR, npm package resolution, QuickJS runtimes, Vue-to-LiveView rendering, and OXC/Vize/Oxide bindings.

Projects:

- **[Volt](https://github.com/elixir-volt/volt)** — Elixir-native frontend build tool: dev server, HMR, Tailwind CSS, JS/TS, Vue/Svelte/React/Solid, and production builds.
- **[QuickBEAM](https://github.com/elixir-volt/quickbeam)** — JavaScript runtime for the BEAM with Web APIs backed by OTP. [Show HN](https://news.ycombinator.com/item?id=47558094)
- **[Phoenix Vapor](https://github.com/elixir-volt/phoenix_vapor)** — Vue templates compiled to native `%Phoenix.LiveView.Rendered{}` structs.
- **[oxc](https://github.com/elixir-volt/oxc_ex)**, **[vize](https://github.com/elixir-volt/vize_ex)**, **[oxide_ex](https://github.com/elixir-volt/oxide_ex)** — Elixir bindings for JS, Vue, and Tailwind toolchains.

## Runtime feedback

- **[pi-elixir](https://github.com/dannote/pi-elixir)** — BEAM runtime tools for [pi](https://github.com/badlogic/pi-mono): eval, docs, process state, Ecto queries, logs, and supervisor trees.
- **[phoenix_replay](https://github.com/dannote/phoenix_replay)** — session recording and replay for Phoenix LiveView.
- **[live_render](https://github.com/dannote/live_render)** — server-driven generative UI for Phoenix LiveView.
- **[phoenix_streamdown](https://github.com/dannote/phoenix_streamdown)** — streaming markdown renderer for Phoenix LiveView, optimized for LLM output. [Hex](https://hex.pm/packages/phoenix_streamdown)

## Agent workflow tools

- **[dot-pi](https://github.com/dannote/dot-pi)** — extensions, skills, and rules for Pi coding agent.
- **[sloplint](https://github.com/dannote/sloplint)** — AST-based multilingual AI slop linter.
- **[agentfmt](https://github.com/dannote/agentfmt)** — token-efficient CLI output formatting for LLM agents.

## Elixir libraries

- **[phoenix_spec](https://github.com/dannote/phoenix_spec)** — OpenAPI 3.1 specs from Phoenix JSON views and Ecto schemas.
- **[json_spec](https://github.com/dannote/json_spec)** — Elixir typespec syntax → JSON Schema, at compile time. [Hex](https://hex.pm/packages/json_spec)
- **[phoenix_iconify](https://github.com/elixir-volt/phoenix_iconify)** / **[iconify](https://github.com/elixir-volt/iconify)** — Iconify SVGs for Elixir, Phoenix, and LiveView. [Hex](https://hex.pm/packages/phoenix_iconify)
- **[qqr](https://github.com/dannote/qqr)** — QR code encoder and decoder in pure Elixir.

## Ruby libraries

- **[typespec_from_serializers](https://github.com/dannote/typespec_from_serializers)** — TypeSpec descriptions from JSON serializers. [RubyGems](https://rubygems.org/gems/typespec_from_serializers)
- **[arel_maniac](https://github.com/dannote/arel_maniac)** — PostgreSQL features for ActiveRecord without raw SQL.

## Search and NLP

- **[Abiko Search](https://github.com/abiko-search)** — search engine for Tor hidden services, built from scratch in Elixir; included an Onion v3 implementation and tor2web proxy. [Product Hunt](https://www.producthunt.com/products/abiko) · [Hacker News](https://news.ycombinator.com/item?id=14927685)
- **[Natasha-Ex](https://github.com/natasha-ex)** — Elixir ports of Russian NLP tools: yargy, slovnet, morph_ru, razmetka, razdel.

## C, Lua, and Linux infrastructure

- **[socks-nginx-module](https://github.com/dannote/socks-nginx-module)** — SOCKS5 proxy support for nginx; referenced on the nginx wiki.
- **[lua-template](https://github.com/dannote/lua-template)** — minimal Lua templating engine adopted by Cloudflare Loom.
- [Xfce garcon desktop actions support](https://gitlab.xfce.org/xfce/garcon/-/commit/aec77533132eb324180ef771e15226a752573eae) — patch to the core Xfce menu library; ships in Xfce since 0.6.0.

## Security research

[Google Bug Hunters](https://bughunters.google.com/profile/62602ae8-cf92-4fb0-810c-c9e284f3427e) · [Bugcrowd](https://bugcrowd.com/h/dannote) · [CodePen Hall of Fame](https://bugcrowd.com/engagements/codepen)
