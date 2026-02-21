# TinyWasm

The TinyWasm project focuses on providing libraries for building applications with web technologies using Go as the main language, compiling to the frontend via WebAssembly with the **minimum possible binary size** (TinyGo compatibility first).

## Why

**Go's WebAssembly potential is incredible**, but traditional applications face a critical challenge: **massive binary sizes** that make web deployment impractical.

### The Problem

Every Go project needs string manipulation, type conversion, and error handling - but importing standard library packages (`fmt`, `strings`, `strconv`, `errors`) creates significant binary bloat that hurts:

- 🌐 **Web app performance** - Slow loading times and poor user experience
- 📱 **Edge deployment** - Resource constraints on small devices
- 🚀 **Distribution efficiency** - Large binaries for simple operations

### The Solution

TinyWasm provides **lightweight, manual implementations** that deliver:

- 🏆 **Drastic size reduction** - Optimized for WebAssembly
- ✅ **Full TinyGo compatibility** - No compilation issues or warnings
- 🎯 **Predictable performance** - No hidden allocations or overhead
- 🔧 **Familiar API** - Drop-in replacement for standard library functions

## Core Framework

The main framework for development is **[tinywasm/app](https://github.com/tinywasm/app)**. It serves as the primary tool for building, watching, and deploying your TinyWasm applications.

## Packages

| Package | Description | Status |
| :--- | :--- | :--- |
| [app](https://github.com/tinywasm/app) | Full stack TUI development environment with live reload, test, deploy, CI/CD for web applications (PWA). | 🚧 In Development |
| [assetmin](https://github.com/tinywasm/assetmin) | A lightweight and efficient web asset packager and minifier for Go applications. | ✅ Ready |
| [binary](https://github.com/tinywasm/binary) | High-performance binary serialization library for Go, specifically designed for TinyGo compatibility. | ✅ Ready |
| [broker](https://github.com/tinywasm/broker) | A lightweight broker that mediates HTTP requests and responses. | 🚧 In Development |
| [bus](https://github.com/tinywasm/bus) | Minimal pub/sub event bus for the tinywasm ecosystem. | ✅ Ready |
| [cdproto](https://github.com/tinywasm/cdproto) | Generated commands, types, and events for the Chrome DevTools Protocol domains. | ✅ Ready |
| [chromedp](https://github.com/tinywasm/chromedp) | A faster, simpler way to drive browsers supporting the Chrome DevTools Protocol. | ✅ Ready |
| [client](https://github.com/tinywasm/client) | Tinywasm compilation toolbox designed to streamline the compilation of Go packages to WebAssembly. | 🚧 In Development |
| [components](https://github.com/tinywasm/components) | HTML components for the go web framework tinywasm. | 🚧 In Development |
| [context](https://github.com/tinywasm/context) | Minimalist context library for TinyGo. | ✅ Ready |
| [crudp](https://github.com/tinywasm/crudp) | A simple binary CRUD protocol for Go structs. | ✅ Ready |
| [crypto](https://github.com/tinywasm/crypto) | CryptoAutoLib port for TinyGo. | ✅ Ready |
| [deploy](https://github.com/tinywasm/deploy) | Automated deployment service for Go applications. | 🚧 In Development |
| [depfind](https://github.com/tinywasm/depfind) | A Go tool to find reverse dependencies - lists packages that import specified target packages. | ✅ Ready |
| [devbrowser](https://github.com/tinywasm/devbrowser) | Lightweight Go library for launching and controlling web browsers programmatically. | ✅ Ready |
| [devflow](https://github.com/tinywasm/devflow) | Complete Go development automation: project init, testing, versioning, updates, and backups. | ✅ Ready |
| [devtui](https://github.com/tinywasm/devtui) | Reusable terminal user interface abstraction for Go development tools. | 🚧 In Development |
| [devwatch](https://github.com/tinywasm/devwatch) | fsnotify implementation that watches file system changes in a project directory. | ✅ Ready |
| [dom](https://github.com/tinywasm/dom) | Ultra-minimal DOM & event toolkit for Go (TinyGo WASM-optimized). | ✅ Ready |
| [fetch](https://github.com/tinywasm/fetch) | A lightweight Go library that unifies HTTP requests across environments. | ✅ Ready |
| [fmt](https://github.com/tinywasm/fmt) | Lightweight Go library that provides comprehensive string manipulation and formatting. | ✅ Ready |
| [form](https://github.com/tinywasm/form) | Form generation using DOM and structs. | 🚧 In Development |
| [gobuild](https://github.com/tinywasm/gobuild) | Minimal build handler for compiling Go or WebAssembly targets via CLI. | ✅ Ready |
| [goflare](https://github.com/tinywasm/goflare) | Lightweight handler for building and deploying Go-based WebAssembly and JavaScript modules to Cloudflare. | 🚧 In Development |
| [gorun](https://github.com/tinywasm/gorun) | Go package to run, monitor, and stop external programs. | ✅ Ready |
| [imagemin](https://github.com/tinywasm/imagemin) | Image size reduction tool for web projects. | ✅ Ready |
| [indexdb](https://github.com/tinywasm/indexdb) | IndexDB implementation with WebAssembly compiled with Go. | 🚧 In Development |
| [json](https://github.com/tinywasm/json) | A lightweight JSON wrapper for Go that optimizes WebAssembly binary size. | ✅ Ready |
| [jsvalue](https://github.com/tinywasm/jsvalue) | Efficient conversions between JavaScript and Go for a WebAssembly environment. | ✅ Ready |
| [keyring](https://github.com/tinywasm/keyring) | A secure credentials manager using DPAPI. | ✅ Ready |
| [kvdb](https://github.com/tinywasm/kvdb) | TinyGo–compatible key–value store with a minimal API. | ✅ Ready |
| [mcp](https://github.com/tinywasm/mcp) | Go implementation of the Model Context Protocol (MCP). | ✅ Ready |
| [mcpserve](https://github.com/tinywasm/mcpserve) | MCP server for TinyWasm ecosystem. | 🚧 In Development |
| [modules](https://github.com/tinywasm/modules) | Common isomorphic modules for SSR and CSR (WebAssembly) compatible with TinyGo. | 🚧 In Development |
| [passkeys](https://github.com/tinywasm/passkeys) | Demo/Example of how to add passkeys. | 🎨 Design |
| [pdf](https://github.com/tinywasm/pdf) | PDF library designed for web rendering with WebAssembly, optimized for TinyGo compatibility. | ✅ Ready |
| [pwa](https://github.com/tinywasm/pwa) | Experimental / Placeholder. | 🎨 Design |
| [rbac](https://github.com/tinywasm/rbac) | RBAC implements Role-Based Access Control to manage roles and permissions. | ✅ Ready |
| [screenshot](https://github.com/tinywasm/screenshot) | Go library to capture desktop to image. | ✅ Ready |
| [server](https://github.com/tinywasm/server) | Go package that encapsulates the logic for running a development and production server. | 🚧 In Development |
| [site](https://github.com/tinywasm/site) | Minimal site rendering engine for Go (WASM-friendly). | 🚧 In Development |
| [sqlite](https://github.com/tinywasm/sqlite) | WebAssembly-first port of modernc.org/sqlite. | 🚧 In Development |
| [sse](https://github.com/tinywasm/sse) | Client and event server, SSE protocol compatible with TinyGo. | ✅ Ready |
| [test-permissions](https://github.com/tinywasm/test-permissions) | Test permissions repository. | 🎨 Design |
| [time](https://github.com/tinywasm/time) | TinyGo-compatible time package for Go. | ✅ Ready |
| [unixid](https://github.com/tinywasm/unixid) | Go library for generating unique, time-based IDs using Unix timestamps. | ✅ Ready |
| [user](https://github.com/tinywasm/user) | User management library. | 🚧 In Development |
| [wasi](https://github.com/tinywasm/wasi) | WASI runtime for tinywasm. | 🚧 In Development |
| [wasmbrowsertest](https://github.com/tinywasm/wasmbrowsertest) | Run WASM tests inside your browser. | ✅ Ready |
| [wizard](https://github.com/tinywasm/wizard) | Modular, pluggable wizard orchestrator for TinyGo applications. | 🚧 In Development |
