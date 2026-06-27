# WookLedger plugin for Claude Code

Adds WookLedger read tools to Claude Code, so your agent can query a WookLedger build while it works: status, verify, audit, checks, savings, receipt, and fleet. Every tool reads local state only and never calls the engine, so nothing leaves your machine.

## Install

```
/plugin marketplace add wookledger/wookledger
/plugin install wookledger@wookledger
```

## Point the tools at your build

By default the tools report on the demo workspace. To monitor a real build, set `WOOK_BUILD_ROOT` to the repo you run `wook build` against. The build-aware tools then report on that build.

## The full tool

WookLedger's core is the `wook` CLI: autonomous, crash-proof, drift-checked builds on your own API key. Get it at wookledger.com.
