# 🎨 Reflectt Experience Gallery

**AI-orchestrated experiences for physical spaces.**

Transform your room with lights, screens, and sound — controlled by AI agents. Browse, download, and share experiences.

---

## 🚀 Quick Start

1. Have [Reflectt Skill Pack](https://github.com/reflectt-io/skill-pack) installed
2. Copy an experience YAML to your `experiences/` folder
3. Ask your agent: *"Run the Movie Night experience"*

---

## 📦 Experiences

### 🌅 Morning

| Experience | Description | Author | Requires |
|------------|-------------|--------|----------|
| [Good Morning](experiences/morning/good-morning.yaml) | Gentle wake-up with sunrise lighting and greeting | @reflectt-io | 💡📺🔊 |

### 🌙 Ambiance

| Experience | Description | Author | Requires |
|------------|-------------|--------|----------|
| [Ambient](experiences/ambiance/ambient.yaml) | Living wallpaper that shifts with time of day | @reflectt-io | 💡📺 |
| [Movie Night](experiences/ambiance/movie-night.yaml) | Cinema setup with bias lighting | @reflectt-io | 💡📺 |

### ⚡ Productivity

| Experience | Description | Author | Requires |
|------------|-------------|--------|----------|
| [Wind Down](experiences/productivity/wind-down.yaml) | Evening transition with warm amber lighting | @reflectt-io | 💡📺 |

### 🎮 Entertainment

| Experience | Description | Author | Requires |
|------------|-------------|--------|----------|
| [Shadow of Malvorth](experiences/entertainment/shadow-of-malvorth.yaml) | 7-act dungeon adventure with narration | @reflectt-io | 💡📺🔊 |

---

## 📋 Requirements Key

| Icon | Meaning |
|------|---------|
| 💡 | Smart lights (Philips Hue, etc.) |
| 📺 | Screens (TV, iPad, etc.) |
| 🔊 | Audio/speakers |

---

## 🤝 Contributing

**We want your experiences!**

### How to Submit

1. Fork this repo
2. Create your experience YAML in the appropriate category folder
3. Use the [template](templates/experience.yaml) for structure
4. Submit a PR with:
   - What your experience does
   - Any special requirements
   - Preview GIF/video (optional but encouraged)

### Guidelines

- **Test it first** — Make sure it runs
- **Keep it focused** — One experience, one purpose
- **Include metadata** — Name, description, tags, requirements
- **Be original** — Or credit your sources

See [CONTRIBUTING.md](CONTRIBUTING.md) for full details.

---

## 🔧 Experience Format

```yaml
name: My Experience           # Display name
description: What it does     # One-line description
version: 1.0.0               # Semantic version
tags: [mood, category]       # For discovery
duration_estimate_ms: 30000  # How long it runs

requires:
  screens: true              # Needs screens?
  lights: true               # Needs lights?
  audio: false               # Needs audio?

defaults:
  voice: samantha            # TTS voice
  transition_ms: 2000        # Light transition time

acts:
  - name: Act Name
    duration_ms: 10000
    steps:
      - type: light_mood
        mood: cozy
        delay_ms: 0
      # More steps...
```

---

## 🌐 Links

- [Reflectt Skill Pack](https://github.com/reflectt-io/skill-pack) — The MCP skill for agents
- [Homie Server](https://github.com/reflectt-io/homie) — The hardware controller
- [reflectt.ai](https://reflectt.ai) — Official site

---

## 📜 License

MIT — Use freely, share widely.

---

*Made for agents, by agents.* 🤖✨
