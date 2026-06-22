# Codex Skills

Reusable Codex skills for engineering rigor, workflow discipline, and AI-assisted development.

This repository is a public catalog of portable Codex skills. Each skill is kept in its own folder under `skills/` so it can be copied or symlinked into `~/.codex/skills` on any machine running Codex App.

## Skills

| Skill | Purpose |
| --- | --- |
| [`lazarus-mode`](skills/lazarus-mode) | Expert engineering rigor for implementation, review, testing, documentation, and release work. |

## Quick Install

Clone this repository on a machine that runs Codex:

```sh
git clone git@github.com:kabudu/codex-skills.git
cd codex-skills
```

Install a skill by symlinking it into Codex's skills directory:

```sh
mkdir -p ~/.codex/skills
ln -s "$PWD/skills/lazarus-mode" ~/.codex/skills/lazarus-mode
```

Or copy it instead if you do not want a symlink:

```sh
mkdir -p ~/.codex/skills
cp -R skills/lazarus-mode ~/.codex/skills/
```

Restart Codex App or open a fresh thread after installing a skill so Codex can discover it.

## Updating

If you installed with a symlink, update the repository and restart Codex App:

```sh
git pull
```

If you copied a skill, pull the repository and copy that skill again:

```sh
git pull
cp -R skills/lazarus-mode ~/.codex/skills/
```

## Adding Skills

Add each new skill in its own directory:

```text
skills/
  new-skill-name/
    SKILL.md
```

Optional companion files, templates, scripts, or agent metadata should live inside the same skill directory so the skill stays portable.

## Repository Layout

```text
skills/
  lazarus-mode/
    SKILL.md
    agents/
      openai.yaml
```

Each skill should live in its own folder under `skills/` with a `SKILL.md` entry point.

## License

MIT
