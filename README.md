<div align="center">

# 🔥 Watchr

### 🚀 The file-watching test runner that never sleeps 🚀

[![Status](https://img.shields.io/badge/Status-🔥%20WORKS-brightgreen?style=for-the-badge)](https://github.com/friuns2/watchr)
[![Ruby](https://img.shields.io/badge/Ruby-💎-cc342d?logo=ruby&logoColor=white&style=for-the-badge)](https://www.ruby-lang.org)
[![Stars](https://img.shields.io/github/stars/friuns2/watchr?style=for-the-badge&logo=github&color=gold)](https://github.com/friuns2/watchr/stargazers)
[![Forks](https://img.shields.io/github/forks/friuns2/watchr?style=for-the-badge&logo=github&color=blue)](https://github.com/friuns2/watchr/network)
[![License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)](LICENSE)

<br />

> **Your filesystem speaks. Watchr listens.**
> **Every save becomes an action. Every change becomes momentum.**

<br />

```
█     █  █████  ██████ ██████ ██  ██ ██████
█     █ ██   ██ █   ██ █      ██  ██ ██   ██
█  █  █ ███████ ██████ █████  ██████ ██████
█ █ █ █ ██   ██ █   ██ █      ██  ██ ██   ██
██   ██ ██   ██ ██████ ██████ ██  ██ ██   ██
```
S P A R K I N G   F A S T   F E E D B A C K

</div>

---

## 🤯 What Is This?
> **The main event.**

Watchr is an agile development tool that **monitors your project tree** and **runs your commands** the instant files change. Think continuous testing, hot feedback loops, and zero patience for slow tooling.

It’s a clean alternative to heavy test runners: **one script, one command, infinite reactions.**

**Yes, it’s a file watcher. Yes, it’s your new test autopilot.**

---

## 🧠 TL;DR
> **The brain-ready summary.**

- 🧪 Write a tiny Ruby script.
- 👂 Watchr listens to file events.
- ⚡ Your tests fire immediately.
- 🏁 You ship faster.

---

## 📱 Demo / Screenshots
> **Proof beats promises.**

No screenshots live in this repo yet. Add them in `images/` and drop them here for instant credibility.

```bash
# ⚡ Run watchr on a script
watchr specs.watchr
```

---

## 🌍 What Can You Do With This?
> **Use cases with zero chill.**

| 🔥 | 🚀 Use Case | 💬 Why It Slaps |
|---|---|---|
| 🧪 | Continuous testing | Tests run on save. No context switch. |
| 🧰 | Scripted workflows | Hook deploys, linters, generators. |
| 🧯 | Hotfix triage | Detect file changes and fire diagnostics. |
| 🧵 | Multi-project monorepos | Watch multiple trees with custom rules. |
| 🎛️ | Tool orchestration | Chain tasks like a lightweight pipeline. |
| 🧹 | Cleanup automation | Auto-delete temp files on changes. |
| ⚙️ | Perf experiments | Re-run benchmarks whenever code shifts. |
| 🧩 | DSL sandboxing | Use the `watch` DSL for custom triggers. |
| 🚦 | CI simulation | Recreate CI steps locally, fast. |
| 🛰️ | Remote dev loops | Watch files on shared mounts. |

---

## ⚡ Quick Start
> **One command to rule them all.**

```bash
# 🔓 Install
gem install watchr

# 🧭 Run a watch script
watchr specs.watchr

# ✅ You are now flying ✈️
```

---

## 📁 Project Structure
> **Know your battlefield.**

```
🧪 specs.watchr      # test watcher rules
📖 docs.watchr       # doc build rules
📦 gem.watchr        # gem packaging rules
🔧 bin/              # CLI entrypoints
🧠 lib/              # core watchr logic
🧾 README.md         # you are here
```

---

## 🧩 The Watch Script DSL
> **Tiny syntax. Huge leverage.**

```ruby
# 👀 Watch tests directly
watch( 'test/test_.*\.rb' ) { |md| system("ruby #{md[0]}") }

# 🔁 Watch libs and run matching tests
watch( 'lib/(.*)\.rb' ) { |md| system("ruby test/test_#{md[1]}.rb") }
```

---

## 🏗️ Architecture
> **Simple pipeline. Loud results.**

```
[Filesystem] --> [Watchr Rules] --> [Action Runner] --> [Test Output]
       |                 |                |                |
      🧩                🧠               ⚙️               ✅
```

---

## 🎯 Requirements
> **Keep it lean.**

- 💎 Ruby (with RubyGems)
- 🧰 Optional: `cool.io` for evented IO on Linux/BSD
- 🍏 Optional: `ruby-fsevent` for OS X file events

---

## 🐛 Troubleshooting
> **Fix it fast.**

| 🧯 Problem | 🛠️ Solution |
|---|---|
| Watchr feels slow | Install `cool.io` or `ruby-fsevent` for native events. |
| Script not firing | Check your regex pattern and file paths. |
| No output | Ensure the command in the block actually runs. |
| Too many triggers | Narrow your watch patterns or debounce. |

---

## 🤝 Contributing
> **PRs are the fuel.**

- 🧱 Open an issue or send a PR on GitHub.
- 🔍 Keep changes small and focused.
- 🧪 Add a test when behavior changes.

---

## ⭐ Star This Repo
> **If this makes your dev loop scream, smash that star button.**

If you believe **fast feedback should be default**, give this repo a star and keep the momentum alive. ⭐

---

<div align="center">
**Built by fearless file watchers** 🔬
*Your code changed. We noticed.* 😏
</div>
