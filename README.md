# Codex Skills

Reusable Codex skills for personal and project workflows.

## Skills

- `lazarus-mode`: Expert engineering rigor for implementation, review, testing, and release work.

## Install A Skill

Clone this repository on a machine that runs Codex:

```sh
git clone git@github.com:kabudu/codex-skills.git
```

Install an individual skill by symlinking it into Codex's skills directory:

```sh
mkdir -p ~/.codex/skills
ln -s "$PWD/skills/lazarus-mode" ~/.codex/skills/lazarus-mode
```

Or copy it instead if you do not want a symlink:

```sh
mkdir -p ~/.codex/skills
cp -R skills/lazarus-mode ~/.codex/skills/
```

Restart Codex App or open a fresh thread after installing a skill.

## Repository Layout

```text
skills/
  lazarus-mode/
    SKILL.md
    agents/
      openai.yaml
```

Each skill should live in its own folder under `skills/` with a `SKILL.md` entry point.
