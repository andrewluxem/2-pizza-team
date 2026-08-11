# 2-pizza-team

A small mission team should contain the fewest dedicated people who can deliver an outcome, learn from it, and make routine decisions without excessive coordination. The label is shorthand for communication discipline, not a literal meal count or a universal headcount rule.

It produces:

- **Team Topology Proposal** (A. Design): built from mission, outcomes, capabilities, capacity, and boundaries.
- **Team Reset Proposal** (B. Reset): built from existing team, observed friction, and changed conditions.
- **Team Topology Audit** (C. Audit): built from current charter, roster by role, decisions, and dependencies.

It executes the [2 Pizza Team playbook](https://www.andrewluxem.com/playbooks/2-pizza-team). The playbook teaches the framework. This skill runs it and returns a working artifact.

**Static by construction: no dependencies, executable code, telemetry, network calls, remote instructions, auto-update, scheduled work, or background behavior.** It reads only the files in its own skill folder. Nothing happens until a user or agent invokes it.

## Install

Clone and copy the skill into Claude Code:

```bash
git clone https://github.com/andrewluxem/2-pizza-team.git
cp -r 2-pizza-team/skills/2-pizza-team ~/.claude/skills/
```

Or install it as a Claude Code plugin:

```text
/plugin marketplace add andrewluxem/2-pizza-team
/plugin install 2-pizza-team@2-pizza-team
```

For clients that install from an archive, keep using the versioned [2-pizza-team v1.0.0 ZIP](https://www.andrewluxem.com/downloads/2-pizza-team-v1.0.0.zip).

## Invoke it

```text
Design team topology for these missions and this headcount
Design team topology for this mission and headcount. The mission is to reduce
Fix this team. It owns acquisition, billing support, and account security.
```

Naming the skill is always valid: `use the 2-pizza-team skill`.

## Files

```text
.claude-plugin/
  plugin.json
  marketplace.json
skills/2-pizza-team/
  SKILL.md
  meta.yaml
  LICENSE.md
  assets/
  references/
README.md
LICENSE
```

The complete canonical package is copied under `skills/2-pizza-team/`, including every asset, reference, example, and license file present in the source.

## Versioning

Plugin installation is version-pinned. When behavior changes, update the version consistently in `SKILL.md`, `meta.yaml`, and `.claude-plugin/plugin.json`, then add a changelog entry. Reinstalling is an explicit update; this repository never auto-updates itself.

## License

MIT. See [LICENSE](LICENSE). The canonical skill folder carries the same authorization in [skills/2-pizza-team/LICENSE.md](skills/2-pizza-team/LICENSE.md).
