# TinyWasm

### Build full-stack web apps in **pure Go** — tiny WebAssembly bundles, zero JS toolchain, built for the age of AI assistants.

TinyWasm is an ecosystem of Go libraries (and a batteries-included dev environment) for building web apps where **Go is the only language** — backend, frontend, and shared logic — compiled to the frontend via WebAssembly with the **smallest possible binary** (TinyGo-first).

👉 **Start here:** [**tinywasm/app**](https://github.com/tinywasm/app) — the TUI dev environment with live reload, MCP for AI assistants, and one-command setup (installation and quick start live there).

---

## Why you might love it

- 🟦 **One language everywhere** — share types, validation, and logic across client and server. No TypeScript, no npm, no bundlers.
- 🪶 **Tiny WASM** — ~200 KB–2 MB depending on mode; TinyGo-first, no hidden allocations.
- 🤖 **Built for AI** — a Model Context Protocol server lets assistants see your UI, read logs, and control compilation.
- 🧰 **Typed construction harness** — APIs designed so the code is easy to read and hard to get wrong: the compiler rejects mistakes, so even an assistant that doesn't know a library builds correctly.
- 🔧 **Zero config** — your project structure *is* the configuration.

## The size problem it solves

Go's WebAssembly potential is huge, but standard-library packages (`fmt`, `strings`, `strconv`, `errors`) bloat binaries — hurting web performance, edge deployment, and distribution. TinyWasm provides **lightweight, TinyGo-compatible implementations** with a familiar API: drastic size reduction, no compilation warnings, predictable performance.

---

## Packages

The libraries you'll use to build apps. The **Activity** badge shows each repo's last commit, pulled live from GitHub — click it to open that library's history.

| Package | Description | Activity |
| :--- | :--- | :--- |
| [app](https://github.com/tinywasm/app) | Full stack TUI development environment with live reload, test, deploy, CI/CD for web applications (PWA). | [![last commit](https://img.shields.io/github/last-commit/tinywasm/app?label=&color=2ea44f)](https://github.com/tinywasm/app/commits) |
| [binary](https://github.com/tinywasm/binary) | High-performance binary serialization library for Go, specifically designed for TinyGo compatibility. | [![last commit](https://img.shields.io/github/last-commit/tinywasm/binary?label=&color=2ea44f)](https://github.com/tinywasm/binary/commits) |
| [components](https://github.com/tinywasm/components) | HTML components for the go web framework tinywasm. | [![last commit](https://img.shields.io/github/last-commit/tinywasm/components?label=&color=2ea44f)](https://github.com/tinywasm/components/commits) |
| [context](https://github.com/tinywasm/context) | Minimalist context library for TinyGo. | [![last commit](https://img.shields.io/github/last-commit/tinywasm/context?label=&color=2ea44f)](https://github.com/tinywasm/context/commits) |
| [crypto](https://github.com/tinywasm/crypto) | CryptoAutoLib port for TinyGo. | [![last commit](https://img.shields.io/github/last-commit/tinywasm/crypto?label=&color=2ea44f)](https://github.com/tinywasm/crypto/commits) |
| [deploy](https://github.com/tinywasm/deploy) | Automated deployment service for Go applications. | [![last commit](https://img.shields.io/github/last-commit/tinywasm/deploy?label=&color=2ea44f)](https://github.com/tinywasm/deploy/commits) |
| [devflow](https://github.com/tinywasm/devflow) | Complete Go development automation: project init, testing, versioning, updates, and backups. | [![last commit](https://img.shields.io/github/last-commit/tinywasm/devflow?label=&color=2ea44f)](https://github.com/tinywasm/devflow/commits) |
| [dom](https://github.com/tinywasm/dom) | Ultra-minimal DOM & event toolkit for Go (TinyGo WASM-optimized). | [![last commit](https://img.shields.io/github/last-commit/tinywasm/dom?label=&color=2ea44f)](https://github.com/tinywasm/dom/commits) |
| [fetch](https://github.com/tinywasm/fetch) | A lightweight Go library that unifies HTTP requests across environments. | [![last commit](https://img.shields.io/github/last-commit/tinywasm/fetch?label=&color=2ea44f)](https://github.com/tinywasm/fetch/commits) |
| [fmt](https://github.com/tinywasm/fmt) | Lightweight Go library that provides comprehensive string manipulation and formatting. | [![last commit](https://img.shields.io/github/last-commit/tinywasm/fmt?label=&color=2ea44f)](https://github.com/tinywasm/fmt/commits) |
| [form](https://github.com/tinywasm/form) | Form generation using DOM and structs. | [![last commit](https://img.shields.io/github/last-commit/tinywasm/form?label=&color=2ea44f)](https://github.com/tinywasm/form/commits) |
| [goflare](https://github.com/tinywasm/goflare) | Lightweight handler for building and deploying Go-based WebAssembly and JavaScript modules to Cloudflare. | [![last commit](https://img.shields.io/github/last-commit/tinywasm/goflare?label=&color=2ea44f)](https://github.com/tinywasm/goflare/commits) |
| [imagemin](https://github.com/tinywasm/imagemin) | Image size reduction tool for web projects. | [![last commit](https://img.shields.io/github/last-commit/tinywasm/imagemin?label=&color=2ea44f)](https://github.com/tinywasm/imagemin/commits) |
| [indexdb](https://github.com/tinywasm/indexdb) | IndexDB implementation with WebAssembly compiled with Go. | [![last commit](https://img.shields.io/github/last-commit/tinywasm/indexdb?label=&color=2ea44f)](https://github.com/tinywasm/indexdb/commits) |
| [json](https://github.com/tinywasm/json) | A lightweight JSON wrapper for Go that optimizes WebAssembly binary size. | [![last commit](https://img.shields.io/github/last-commit/tinywasm/json?label=&color=2ea44f)](https://github.com/tinywasm/json/commits) |
| [jsvalue](https://github.com/tinywasm/jsvalue) | Efficient conversions between JavaScript and Go for a WebAssembly environment. | [![last commit](https://img.shields.io/github/last-commit/tinywasm/jsvalue?label=&color=2ea44f)](https://github.com/tinywasm/jsvalue/commits) |
| [kvdb](https://github.com/tinywasm/kvdb) | TinyGo–compatible key–value store with a minimal API. | [![last commit](https://img.shields.io/github/last-commit/tinywasm/kvdb?label=&color=2ea44f)](https://github.com/tinywasm/kvdb/commits) |
| [mcp](https://github.com/tinywasm/mcp) | Go implementation of the Model Context Protocol (MCP). | [![last commit](https://img.shields.io/github/last-commit/tinywasm/mcp?label=&color=2ea44f)](https://github.com/tinywasm/mcp/commits) |
| [pdf](https://github.com/tinywasm/pdf) | PDF library designed for web rendering with WebAssembly, optimized for TinyGo compatibility. | [![last commit](https://img.shields.io/github/last-commit/tinywasm/pdf?label=&color=2ea44f)](https://github.com/tinywasm/pdf/commits) |
| [postgres](https://github.com/tinywasm/postgres) | PostgreSQL adapter implementing the `tinywasm/orm` Adapter interface. | [![last commit](https://img.shields.io/github/last-commit/tinywasm/postgres?label=&color=2ea44f)](https://github.com/tinywasm/postgres/commits) |
| [sqlite](https://github.com/tinywasm/sqlite) | WebAssembly-first port of modernc.org/sqlite. | [![last commit](https://img.shields.io/github/last-commit/tinywasm/sqlite?label=&color=2ea44f)](https://github.com/tinywasm/sqlite/commits) |
| [sse](https://github.com/tinywasm/sse) | Client and event server, SSE protocol compatible with TinyGo. | [![last commit](https://img.shields.io/github/last-commit/tinywasm/sse?label=&color=2ea44f)](https://github.com/tinywasm/sse/commits) |
| [time](https://github.com/tinywasm/time) | TinyGo-compatible time package for Go. | [![last commit](https://img.shields.io/github/last-commit/tinywasm/time?label=&color=2ea44f)](https://github.com/tinywasm/time/commits) |
| [unixid](https://github.com/tinywasm/unixid) | Go library for generating unique, time-based IDs using Unix timestamps. | [![last commit](https://img.shields.io/github/last-commit/tinywasm/unixid?label=&color=2ea44f)](https://github.com/tinywasm/unixid/commits) |
| [user](https://github.com/tinywasm/user) | User management library. | [![last commit](https://img.shields.io/github/last-commit/tinywasm/user?label=&color=2ea44f)](https://github.com/tinywasm/user/commits) |

---

## Get involved

We're building a **Go-first web ecosystem** and welcome contributions — Go ports of browser APIs, performance tools, starter templates, docs, and bug reports.

- 💬 [Discussions](https://github.com/tinywasm/app/discussions) · 🐞 [Issues](https://github.com/tinywasm/app/issues)
- ⭐ Star the libraries you find useful — it helps others discover the ecosystem.
