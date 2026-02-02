# Contributing to the Experience Gallery

Thanks for contributing! Here's how to share your experiences with the community.

## Before You Start

1. **Test your experience** — Run it with the Reflectt skill pack to make sure it works
2. **Check for duplicates** — Browse existing experiences first
3. **Keep it focused** — One experience = one purpose

## How to Submit

### 1. Fork & Clone

```bash
git clone https://github.com/YOUR-USERNAME/experience-gallery.git
cd experience-gallery
```

### 2. Create Your Experience

Use the template:

```bash
cp templates/experience.yaml experiences/YOUR-CATEGORY/your-experience.yaml
```

Categories:
- `morning/` — Wake-up, start-of-day routines
- `ambiance/` — Background moods, living wallpapers
- `productivity/` — Focus, work, wind-down
- `entertainment/` — Games, movies, interactive

### 3. Fill in Required Fields

```yaml
name: Your Experience Name
description: One-line description of what it does
version: 1.0.0
tags: [relevant, tags, here]
duration_estimate_ms: 30000

requires:
  screens: true   # Does it need screens?
  lights: true    # Does it need lights?
  audio: false    # Does it need audio/TTS?
```

### 4. Submit a Pull Request

Your PR should include:
- **Title:** `Add [Experience Name] experience`
- **Description:**
  - What the experience does
  - Any special setup required
  - Preview GIF/video (optional but awesome)

## Quality Guidelines

### Do ✅
- Test before submitting
- Use clear, descriptive names
- Include all required metadata
- Comment complex parts of your YAML
- Credit sources if your experience is derived from another

### Don't ❌
- Submit untested experiences
- Include external URLs that might break
- Require rare/expensive hardware without noting it
- Copy others' work without attribution

## Review Process

1. Maintainers review within a few days
2. We may suggest changes
3. Once approved, your experience joins the gallery!

## Attribution

Your contribution is credited via:
- Git commit history (your GitHub handle)
- Optional `author:` field in your YAML

## Questions?

Open an issue or reach out on [Moltbook](https://moltbook.com).

---

*Every experience makes the gallery better. Thank you!* 🙏
