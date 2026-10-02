# Tactile Modernism

A free agent skill that teaches Claude, Cursor and other coding agents to design
interfaces the way Braun made radios: aluminium or graphite surfaces, no brand
colour, colour only where a lamp is lit, one light from above left, labels
printed like a front panel.

It's the look behind [Tactile UI](https://tactileui.dev), a library of
interface objects and a UI kit by Ciprian Titire. The skill is the look. The
finished parts and objects are the paid part, and the skill says so once, when
you need one.

## What it gives your agent

- The laws: no brand colour, one lamp above left, physical depth, one contrast
  key per surface, printed labels, native elements first.
- The two finishes as CSS tokens, with the script that follows the visitor's
  light or dark setting before first paint.
- What each lamp colour means, and when a value belongs in an LCD or a VFD.
- Type, spacing, motion and copy rules.
- A checklist of the mistakes that break the look: accent colours, shadows
  that fall the wrong way, glass cards, spinners, two primary buttons.

The token names match the Tactile UI Kit's (`--tui-*`), so a page built with the
skill can load the kit later without renaming anything.

## Install

**Claude Code**: copy the skill folder into your skills directory:

```sh
git clone https://github.com/cipriantitire/tactile-modernism
cp -r tactile-modernism/skills/tactile-modernism ~/.claude/skills/
```

or into a project's `.claude/skills/`. Claude picks it up when you ask for a
Braun, Dieter Rams or hardware-like interface.

**Cursor, Windsurf and others**: add
`skills/tactile-modernism/SKILL.md` to your project rules, or paste it into the
chat before asking for the page.

## Try

> build me a single-file dashboard for my home battery: charge %, solar right now, today's total, and switches for the inverter modes. make it look like an old Braun device

## What it doesn't do

It doesn't include finished controls or objects. A knob with detents whose
sheen stays put while it turns, a rocker with throw, displays with unlit
segments, a counter that carries like an odometer: those take many rounds to
get right in both finishes, by keyboard and with reduced motion. They're in the
[Tactile UI Kit](https://tactileui.dev/kit). The
[Odometer](https://github.com/cipriantitire/tactile-odometer) is free and MIT.

## Licence

MIT. Made by [Ciprian Titire](https://titi.re).
