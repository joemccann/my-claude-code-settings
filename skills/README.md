# Skills

This directory contains skill definitions for Claude Code.

## For Pre-Built/Custom Skills (Manual Upload)

1. Enable Code Execution: In Claude, go to Settings > Capabilities and ensure "Code execution and file creation" is on.
2. Locate Skills Folder: Create the directory `~/.claude/skills/` (or `.claude/skills/` inside a specific project).
3. Get the Skill File: Create a folder with a `SKILL.md` file inside your skills directory (e.g., `~/.claude/skills/my-skill/SKILL.md`).
4. Place your skill's folder (containing `SKILL.md`) directly into the `~/.claude/skills/` folder.
5. Activate: Toggle the skill on in Settings > Capabilities > Skills.

## Usage

Start a new chat and prompt Claude to use your skill, e.g., "Use the 'My Skill' to...". 

## For Creating Skills with Claude

1. Enable Skill Creator: Turn on the "skill-creator" skill in Settings > Capabilities > Skills.
2. Start Creation: Open a chat and ask Claude to use the "skill-creator" to build a new skill, describing your desired functionality.
3. Review & Download: Claude will generate the skill files (including `SKILL.md`) and a `README.md`. Download these.
4. Install: Follow the steps above to upload or place the generated skill files into your skills directory and activate it. 

## Key Concepts

- Progressive Disclosure: Claude only loads skills it deems relevant based on your prompt and the skill's description in `SKILL.md`.
- `SKILL.md`: The core of a skill, containing metadata (name, description) and instructions for Claude.
- Security: Only install skills from trusted sources, as they can execute code. 