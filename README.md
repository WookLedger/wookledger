# WookLedger

Durable, verified, crash-proof state for AI coding agents.

State lives in durable files, so a crash, a timeout, or a usage-limit stop resumes from the exact cursor with nothing redone. Every change is verified after the fact, with drift caught at the exact line, and work is never marked done until your own check passes. You run the model on your own key; the orchestration method stays server-side and never ships to your machine.

## Install in Claude Code

```
/plugin marketplace add wookledger/wookledger
/plugin install wookledger@wookledger
```

This adds read tools (status, verify, audit, checks, savings, receipt, fleet) that query your build's ledger, integrity, and savings while the agent works. The tools read local state only and never call the engine, so nothing leaves your machine.

## The full tool

The plugin adds in-editor read tools. WookLedger's core is the `wook` CLI, which runs the autonomous, crash-proof, drift-checked builds on your own API key. Get it at wookledger.com.

## What ships here

The thin client only: an MCP server bundled to one self-contained file, with the wook CLI bundled beside it for the server to run. The proprietary method never ships.
